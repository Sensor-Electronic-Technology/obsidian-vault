testing to make sure changes sync

```csharp title="SignalR HTTPS Cert"
    private static void SignalRCertVerification(HttpConnectionOptions options) {
        var companyRootCA = new X509Certificate2("/secrets/certs/tls.crt");
        Func<object, X509Certificate?, X509Chain?, System.Net.Security.SslPolicyErrors, bool>
            customValidator =
                (sender, certificate, chain, sslPolicyErrors) => {
                    if (chain == null || certificate == null) return false;
                    chain.ChainPolicy.ExtraStore.Add(companyRootCA);
                    chain.ChainPolicy.VerificationFlags =
                        X509VerificationFlags.AllowUnknownCertificateAuthority;
                    var element = new X509Certificate2(certificate);
                    bool isValidChain = chain.Build(element);
                    bool matchesCompanyRoot = chain.ChainElements[^1].Certificate.Thumbprint ==
                                              companyRootCA.Thumbprint;
                    return isValidChain && matchesCompanyRoot;
                };
        options.HttpMessageHandlerFactory = (innerHandler) => {
            if (innerHandler is HttpClientHandler clientHandler) {
                clientHandler.ServerCertificateCustomValidationCallback =
                    (m, c, ch, e) => customValidator(m, c, ch, e);
            }

            return innerHandler;
        };
        options.WebSocketConfiguration = (webSocketOptions) => {
            webSocketOptions.RemoteCertificateValidationCallback =
                (s, c, ch, e) => customValidator(s, c, ch, e);
        };
    }
```


```bash title:"Initialize Repo"
git init -b main
git commit -m "Initial Commit"
gh repo create Sensor-Electronic-Technology/obsidian-vault --source=. --public --push
nano .gitignore
# add folder (anywhere)/folder-to-ignore/ or foler-to-ignore/
git add .gitignore
git commit -m "Add gitignore"
## if folder is already in commit
git rm -r --cached folder-to-ignore/
git commit -m "remove folder from repo"
gh repo sync -force
```


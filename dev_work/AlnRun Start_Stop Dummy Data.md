# Run 1 Dummy Data

```json title="StartAlnRunCommand"
{
  "wafers": [
    {
      "rlWaferId": null,
      "runId": "A99-0001",
      "sapphireVendor": "jshine",
      "sapphireSubstrate": "pss",
      "growthDate": "2026-09-23T10:54:45.099571+00:00",
      "reactor": "A99",
      "runType": "RL",
      "waferId": "A99-0001-01"
    },
    {
      "rlWaferId":null,
      "runId": "A99-0001",
      "sapphireVendor": "jshine",
      "sapphireSubstrate": "pss",
      "growthDate": "2026-09-23T10:54:45.099571+00:00",
      "reactor": "A99",
      "runType": "RL",
      "waferId": "A99-0001-02"
    },
    {
      "rlWaferId":null,
      "runId": "A99-0001",
      "sapphireVendor": "jshine",
      "sapphireSubstrate": "pss",
      "growthDate": "2026-09-23T10:54:45.099571+00:00",
      "reactor": "A99",
      "runType": "RL",
      "waferId": "A99-0001-03"
    }
  ],
  "addToQueue": false,
  "moData": {
    "_t": "mo-data-a-dto",
    "tmAl1Temp": 35,
    "tmAl1Weight": 456,
    "additionalData": {}
  },
  "additionalData": {},
  "epiThickness": "A",
  "sapThickness": "B01",
  "substrate": "2",
  "process": "1",
  "isAnnealed": false,
  "growthDate": "2026-09-23T10:54:45.099571+00:00",
  "systemType": "ASystem",
  "reactor": "A99",
  "technician": "AE",
  "waferSize": "2",
  "runType": "RL",
  "subRunType": "something-other",
  "structure": "something",
  "projectCode": "P0123452",
  "recipe": null,
  "hasStock": true,
  "beforeCheckList": [
    {
      "name": "",
      "description": "",
      "completed": true
    }
  ],
  "afterCheckList": [
    {
      "name": "",
      "description": "",
      "completed": true
    }
  ],
  "generalCheckList": [
    {
      "name": "",
      "description": "",
      "completed": true
    }
  ],
  "modifiedBy": {
    "userID": "aelmendorf",
    "userName":"aelmendo"
  },
  "waferRunId": "A99-0001"
}
```

```json title:"StopAlnRunCommand"
{
  "growthRunMonitorDto": {
    "_t": "system-a-monitor-log",
    "lowTempRegion": {
      "additionalData": {},
      "rfUPercent": 1,
      "rfPower": 1,
      "reactorTemp": 1,
      "epiTemp1": 1,
      "epiTemp7": 1,
      "epiTemp12": 1,
      "ceilingTemp": 1,
      "centerLoopTemp": 1,
      "pressure": 1,
      "throttleValvePosPercent": 1,
      "dorPressure": 1
    },
    "highTempRegion": {
      "additionalData": {},
      "rfUPercent": 1,
      "rfPower": 1,
      "reactorTemp": 1,
      "epiTemp1": 1,
      "epiTemp7": 1,
      "epiTemp12": 1,
      "ceilingTemp": 1,
      "centerLoopTemp": 1,
      "pressure": 1,
      "throttleValvePosPercent": 1,
      "dorPressure": 1
    },
    "growthDate": "2026-09-23T15:54:45.099571+00:00",
    "modifiedBy": {
      "userID": "aelmendorf",
      "userName": "aelmendo"
    },
    "waferRunId": "A99-0001",
    "additionalData": {}
  },
  "moData": {
    "_t": "mo-data-a-dto",
    "tmAl1Temp": 32,
    "tmAl1Weight": 875,
    "additionalData": {}
  },
  "runEnd": "2026-09-23T15:54:45.099571+00:00",
  "modifiedBy": {
    "userID": "aelmendorf",
    "userName":"aelmendo"
  },
  "waferRunId": "A99-0001"
}
```

---
# Run 2 Dummy Data

```json title="StartAlnRunCommand"
{
  "wafers": [
    {
      "rlWaferId": null,
      "runId": "A99-0002",
      "sapphireVendor": "jshine",
      "sapphireSubstrate": "pss",
      "growthDate": "2026-09-23T10:54:45.099571+00:00",
      "reactor": "A99",
      "runType": "RL",
      "waferId": "A99-0002-01"
    },
    {
      "rlWaferId":null,
      "runId": "A99-0002",
      "sapphireVendor": "jshine",
      "sapphireSubstrate": "pss",
      "growthDate": "2026-09-23T10:54:45.099571+00:00",
      "reactor": "A99",
      "runType": "RL",
      "waferId": "A99-0002-02"
    },
    {
      "rlWaferId":null,
      "runId": "A99-0002",
      "sapphireVendor": "jshine",
      "sapphireSubstrate": "pss",
      "growthDate": "2026-09-23T10:54:45.099571+00:00",
      "reactor": "A99",
      "runType": "RL",
      "waferId": "A99-0002-03"
    }
  ],
  "addToQueue": false,
  "moData": {
    "_t": "mo-data-a-dto",
    "tmAl1Temp": 35,
    "tmAl1Weight": 456,
    "additionalData": {}
  },
  "additionalData": {},
  "epiThickness": "A",
  "sapThickness": "B01",
  "substrate": "2",
  "process": "1",
  "isAnnealed": false,
  "growthDate": "2026-09-23T10:54:45.099571+00:00",
  "systemType": "ASystem",
  "reactor": "A99",
  "technician": "AE",
  "waferSize": "2",
  "runType": "RL",
  "subRunType": "something-other",
  "structure": "something",
  "projectCode": "P0123452",
  "recipe": null,
  "hasStock": true,
  "beforeCheckList": [
    {
      "name": "",
      "description": "",
      "completed": true
    }
  ],
  "afterCheckList": [
    {
      "name": "",
      "description": "",
      "completed": true
    }
  ],
  "generalCheckList": [
    {
      "name": "",
      "description": "",
      "completed": true
    }
  ],
  "modifiedBy": {
    "userID": "aelmendorf",
    "userName":"aelmendo"
  },
  "waferRunId": "A99-0002"
}
```

```json title="StopAlnRunCommand"
{
  "growthRunMonitorDto": {
    "_t": "system-a-monitor-log",
    "lowTempRegion": {
      "additionalData": {},
      "rfUPercent": 1,
      "rfPower": 1,
      "reactorTemp": 1,
      "epiTemp1": 1,
      "epiTemp7": 1,
      "epiTemp12": 1,
      "ceilingTemp": 1,
      "centerLoopTemp": 1,
      "pressure": 1,
      "throttleValvePosPercent": 1,
      "dorPressure": 1
    },
    "highTempRegion": {
      "additionalData": {},
      "rfUPercent": 1,
      "rfPower": 1,
      "reactorTemp": 1,
      "epiTemp1": 1,
      "epiTemp7": 1,
      "epiTemp12": 1,
      "ceilingTemp": 1,
      "centerLoopTemp": 1,
      "pressure": 1,
      "throttleValvePosPercent": 1,
      "dorPressure": 1
    },
    "growthDate": "2026-09-23T15:54:45.099571+00:00",
    "modifiedBy": {
      "userID": "aelmendorf",
      "userName": "aelmendo"
    },
    "waferRunId": "A99-0002",
    "additionalData": {}
  },
  "moData": {
    "_t": "mo-data-a-dto",
    "tmAl1Temp": 32,
    "tmAl1Weight": 875,
    "additionalData": {}
  },
  "runEnd": "2026-09-23T15:54:45.099571+00:00",
  "modifiedBy": {
    "userID": "aelmendorf",
    "userName":"aelmendo"
  },
  "waferRunId": "A99-0002"
}
```


---

# skydash

This repository contains a simple model in c# of the response from Skyscape when querying their API to retrieve detail on your VApps and VMs.

https://portal.skyscapecloud.com/api/my_vm

The project contains a sample response from this endpoint in a json file "data.json". To convert the raw string response from the API, simply use:

```c#
var result = JsonConvert.DeserializeObject<Dictionary<string, VAppAndMachineWrapper>>(json);
```

# StartESX
Start ESX with a line, dont need any return, all will be done automatically.<br>
It also automatically loads player data (like the job, that auto update) 

the `ESX` variables are made available

| Argument              | Data Type                            | Nedeed                    | Default                       | Description
| ----------------------| ------------------------------------ | ------------------------- |-------------------------------|-------------
| `esxEventName`                | string | :material-checkbox-blank-circle-outline: | `esx:getSharedObject` | The esx event, if you have the replaced trigger
| `Second Job`                | string | :material-checkbox-blank-circle-outline: | `-` | If you have set up the second job in the utility configuration, you need to enter the name here for it to auto-update

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    StartESX()
    ```     

??? abstract "Old method"
    ```
    ESX = nil
    TriggerEvent('esx:getSharedObject', function(obj) ESX = obj end)
    ```

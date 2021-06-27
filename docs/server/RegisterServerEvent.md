# RegisterServerEvent
Register a server event that can be called by the client or the server,<br>**The event have the AddEventHandler already loaded**

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `EventName`                | string | :material-checkbox-blank-circle: | `-` | The name of the event
| `Function`                | function | :material-checkbox-blank-circle: | `-` | The code executed when the event was triggered
| `Auto-Prepare`                | boolean | :material-checkbox-blank-circle-outline: | `true` | If setted to false dont auto-prepare the event for works with ESX (dont load the esx basic variable)

???+ info "Other difference"
    It also auto-prepare the event to work with esx, so it auto load the `xPlayer` and `_source` variable

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    RegisterServerEvent("utility_libs:ILoveYou", function()
        print(GetPlayerName().." love the utility_libs, how to blame it?")
    end)
    ```
??? abstract "Old method"
    ```
    RegisterServerEvent("utility_libs:ILoveYou")
    AddEventHandler("utility_libs:ILoveYou", function()
        local _source = source
        local xPlayer = ESX.GetPlayerFromId(_source)

        print(GetPlayerName(PlayerId()).." love the utility_libs, how to blame it?")
    end)
    ```
    ??? info "Using old native"
        although i dont recommend it, you can use the old native via `old_RegisterServerEvent`
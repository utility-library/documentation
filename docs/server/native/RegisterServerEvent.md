# RegisterServerEvent
Record a server-side event that is triggerable by the server and also by the client.<br>**The event have the AddEventHandler already loaded**

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `EventName`                | string | :material-checkbox-blank-circle: | `-` | The name of the event
| `Function`                | function | :material-checkbox-blank-circle: | `-` | The code executed when the event was triggered
| `Auto-Prepare`                | boolean | :material-checkbox-blank-circle-outline: | `true` | If setted to false don't auto-prepare the event for works with ESX (don't load the esx basic variable)

???+ info "Other difference"
    It also auto-prepare the event to work with esx, so it auto load the `xPlayer` and `_source` variable

!!! success ""
    Don't need to be called every frame
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
        although i don't recommend it, you can use the old native via `old_RegisterServerEvent`
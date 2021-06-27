# RegisterNetEvent
Register a net event that can be called by the client or the server,<br>**The event have the AddEventHandler already loaded**

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `EventName`                | string | :material-checkbox-blank-circle: | `-` | The name of the event
| `Function`                | function | :material-checkbox-blank-circle: | `-` | The code executed when the event was triggered

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    RegisterNetEvent("utility_libs:ILoveYou", function()
        print(GetPlayerName().." love the utility_libs, how to blame it?")
    end)
    ```
??? abstract "Old method"
    ```
    RegisterNetEvent("utility_libs:ILoveYou")
    AddEventHandler("utility_libs:ILoveYou", function()
        print(GetPlayerName(PlayerId()).." love the utility_libs, how to blame it?")
    end)
    ```
    ??? info "Using old native"
        although i dont recommend it, you can use the old native via `old_RegisterNetEvent`
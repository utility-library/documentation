# TriggerSyncedEvent (Client side)
Trigger a net event for all clients

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `EventName`                | string | :material-checkbox-blank-circle: | `-` | The net event name
| `Whitelist`                | number/table | :material-checkbox-blank-circle: | `-` | This is the whitelist, for each id the defined event will be triggered, insert **-1** for trigger the event for any client or create a table with all the id
| `Any other argument`                | any | :material-checkbox-blank-circle-outline: | `-` | You can pass any argument, its equal to the Trigger

!!! success ""
    Dont need to be called every frame
---
??? example
    ??? note "If we want to trigger the event for any client"
        ```
        RegisterNetEvent("utility_libs:ILoveYou", function()
            print("i love the utility_libs")
        end)

        TriggerSyncedEvent("utility_libs:ILoveYou", -1)
        ```
        ??? success "Expected Results"
            **ID 1**: i see the message "i love the utility_libs"<br>
            **ID 2**: i see the message "i love the utility_libs"<br>
            **ID 3**: i see the message "i love the utility_libs"<br>
            ...etc
    ??? note "Or if we want to trigger the event only for id 1 and 2"
        ```
        RegisterNetEvent("utility_libs:ILoveYou", function()
            print("i love the utility_libs")
        end)

        TriggerSyncedEvent("utility_libs:ILoveYou", {1,2})
        ```
        ??? success "Expected Results"
            **ID 1**: i see the message "i love the utility_libs"<br>
            **ID 2**: i see the message "i love the utility_libs"<br>
            **ID 3**: i dont see any message        

??? abstract "Old method"
    Client:
    ```
    RegisterNetEvent("utility_libs:ILoveYou")
    AddEventHandler("utility_libs:ILoveYou", function()
        print("i love the utility_libs")
    end)

    TriggerServerEvent("utility_libs:ILoveYou_S")
    ```
    Server:
    ```
    RegisterServerEvent("utility_libs:ILoveYou_S")
    AddEventHandler("utility_libs:ILoveYou_S", function()
        TriggerClientEvent("utility_libs:ILoveYou", -1)
    end)
    ```

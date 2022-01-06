# Synced [BETA]
Create a synced variable, the synced variable is a variable that is synchronized with all other clients, a flowdetector is integrated directly into the synced variable, so when the data will change the variable will be automatically resynchronized with all clients, can be very useful to create scripts for lobbies or for anything else that requires that a variable is the same for all clients

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `name`                | string | :material-checkbox-blank-circle: | `-` | The variable name
| `value`                | anything | :material-checkbox-blank-circle: | `-` | The value of the variable

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    Synced("mydata", "Im blank")

    RegisterCommand("changedata", function()
        mydata = "Utility"
    end)

    RegisterCommand("isynced", function()
        print(mydata)
    end)
    ```

    So if ID 1 do the command "changedata"<br>
    And another player does the "issynced" command in the client console will come out "Utility"
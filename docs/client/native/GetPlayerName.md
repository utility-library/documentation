# GetPlayerName
Returns the player name, the difference between the standrard one and this one is that this one have the playerid has default

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `PlayerId`                | number | :material-checkbox-blank-circle-outline: | `playerId` | The local player id

??? success "Returns"
    | Data Type                            | Description
    | ------------------------------------ |-------------
    | name | The player name
    
!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    GetPlayerName()
    ```
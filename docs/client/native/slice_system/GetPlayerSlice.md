# GetPlayerSlice
Get the slice id from a player index (client id)

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `player`                | Player | :material-checkbox-blank-circle: | `-` | The player that whe need to get the slice id

??? success "Returns"
    | Data Type                            | Description
    | ------------------------------------ |-------------
    | number | The slice id

---
??? example
    ```
    local slice = GetPlayerSlice(PlayerId())

    print("Current slice: "..slice)
    ```
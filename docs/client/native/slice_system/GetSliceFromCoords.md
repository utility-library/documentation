# GetSliceFromCoords
Get the slice id from some coords

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `coords`                | vector3 | :material-checkbox-blank-circle: | `-` | The coords of where whe need to get the slice id

??? success "Returns"
    | Data Type                            | Description
    | ------------------------------------ |-------------
    | number | The slice id

---
??? example
    ```
    local playerCoords = GetEntityCoords(PlayerPedId())
    local slice = GetSliceFromCoords(playerCoords)

    print("Current slice: "..slice)
    ```
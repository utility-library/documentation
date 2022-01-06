# GetSliceCoordsFromCoords
Get the slice coords from a coords

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `coords`                | vector3 | :material-checkbox-blank-circle: | `-` | The coords of where whe need to get the coords

??? success "Returns"
    | Data Type                            | Description
    | ------------------------------------ |-------------
    | vector2 | The x and the y of the center of the slice

---
??? example
    ```
    local playerCoords = GetEntityCoords(PlayerPedId())
    local slice = GetSliceCoordsFromCoords(playerCoords)

    print("The center of that slice is "..slice)
    ```
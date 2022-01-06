# GetEntitySlice
Get the slice id from a entity

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `entity`                | entity | :material-checkbox-blank-circle: | `-` | The entity that whe need to get the slice id

??? success "Returns"
    | Data Type                            | Description
    | ------------------------------------ |-------------
    | number | The slice id

---
??? example
    ```
    local slice = GetEntitySlice(PlayerPedId())

    print("Current slice: "..slice)
    ```
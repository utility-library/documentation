# SocietyHaveItemQuantity
Check if the society inventory have that item quantity

| Argument              | Data Type                            | Needed                    | Default                       | Description
| ----------------------| ------------------------------------ | ------------------------- |-------------------------------|-------------
| `Society`                | string | :material-checkbox-blank-circle: | `-` | The society name
| `Item`                | string | :material-checkbox-blank-circle: | `-` | The item name
| `Quantity`                | number | :material-checkbox-blank-circle: | `-` | The item quantity

!!! success ""
    Dont need to be called every frame

??? success "Returns"
    | Data Type | Description                           |
    |-----------|---------------------------------------|
    | boolean   | If have or no the item quantity                          |


---
??? example
    ```
    local have_item = SocietyHaveItemQuantity("police", "bread", 3)
    ```
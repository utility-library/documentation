# HaveItemQuantity
Check if the player have that item quantity

| Argument              | Data Type                            | Nedeed                    | Default                       | Description
| ----------------------| ------------------------------------ | ------------------------- |-------------------------------|-------------
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
    local have_item = HaveItemQuantity("bread", 3)
    ```
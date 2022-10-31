# HaveItem
Check if the player have that item

| Argument              | Data Type                            | Needed                    | Default                       | Description
| ----------------------| ------------------------------------ | ------------------------- |-------------------------------|-------------
| `id`                | number | :material-checkbox-blank-circle: | `-` |
| `Item`                | string | :material-checkbox-blank-circle: | `-` | The item name

!!! success ""
    Dont need to be called every frame

??? success "Returns"
    | Data Type | Description                           |
    |-----------|---------------------------------------|
    | boolean   | If have or no the item                           |


---
??? example
    ```
    local have_item = HaveItem(source, "bread")
    ```
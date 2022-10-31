# GetItem
Get data of an item by the player

| Argument              | Data Type                            | Needed                    | Default                       | Description
| ----------------------| ------------------------------------ | ------------------------- |-------------------------------|-------------
| `id`                | number | :material-checkbox-blank-circle: | `-` |
| `Item`                | string | :material-checkbox-blank-circle: | `-` | The item name

!!! success ""
    Dont need to be called every frame

??? success "Returns"
    | Child     | Data Type | Description                           |
    |-----------|-----------|---------------------------------------|
    | name      | string    | Item name                             |
    | count     | number    | Item count                            |
    | label     | string    | Item label                            |
    | weight    | number    | Item weight                           |
    | usable    | boolean   | Whether or not the item is usable     |
    | rare      | boolean   | Whether or not the item is rare       |
    | canRemove | boolean   | Whether or not the item can be thrown |



---
??? example
    ```
    local itemData = GetItem(source, "bread")
    ```     
    How to use child
    ```
    local itemData = GetItem(source, "bread")

    -- itemData.name = "bread"
    -- itemData.count = 1
    -- ...
    ```
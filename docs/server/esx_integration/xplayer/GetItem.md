# GetItem
Get data of an item by the player

| Argument              | Data Type                            | Needed                    | Default                       | Description
| ----------------------| ------------------------------------ | ------------------------- |-------------------------------|-------------
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
    local itemData = GetItem("bread")
    ```     
    How to use child
    ```
    local itemData = GetItem("bread")

    -- itemData.name = "bread"
    -- itemData.count = 1
    -- ...
    ```
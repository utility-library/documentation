# SocietyGetItem
Get data of an item from the society inventory

| Argument              | Data Type                            | Nedeed                    | Default                       | Description
| ----------------------| ------------------------------------ | ------------------------- |-------------------------------|-------------
| `Society`                | string | :material-checkbox-blank-circle: | `-` | The society name
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
    local itemData = SocietyGetItem("police", "bread")
    ```     
    How to use child
    ```
    local itemData = SocietyGetItem("police", "bread")

    -- itemData.name = "bread"
    -- itemData.count = 1
    -- ...
    ```
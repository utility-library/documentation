# SocietyRemoveItem
Remove an item from the society inventory

| Argument              | Data Type                            | Nedeed                    | Default                       | Description
| ----------------------| ------------------------------------ | ------------------------- |-------------------------------|-------------
| `Society`                | string | :material-checkbox-blank-circle: | `-` | The society name
| `Item`                | string | :material-checkbox-blank-circle: | `-` | The item name
| `Amount`                | number | :material-checkbox-blank-circle: | `-` | The amount

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    SocietyRemoveItem("police", "bread", 1)
    ```     

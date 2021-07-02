# RemoveItem (Client side)
Remove an item from the player

| Argument              | Data Type                            | Nedeed                    | Default                       | Description
| ----------------------| ------------------------------------ | ------------------------- |-------------------------------|-------------
| `Item`                | string | :material-checkbox-blank-circle: | `-` | The item name
| `Amount`                | number | :material-checkbox-blank-circle: | `-` | The amount

???+ warning
    For server safety, the trigger below the function can be disabled in the utility config

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    RemoveItem("bread", 1)
    ```     

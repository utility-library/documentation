# AddItem
Add an item to the player

| Argument | Data Type | Needed                           | Default | Description   |
|----------|-----------|----------------------------------|---------|---------------|
| `id`     | number    | :material-checkbox-blank-circle: | `-`     |               |
| `Item`   | string    | :material-checkbox-blank-circle: | `-`     | The item name |
| `Amount` | number    | :material-checkbox-blank-circle: | `-`     | The amount    |

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    AddItem(source, "bread", 1)
    ```     

# SocietyAddItem
Add an item to the society inventory

| Argument              | Data Type                            | Needed                    | Default                       | Description
| ----------------------| ------------------------------------ | ------------------------- |-------------------------------|-------------
| `Society`                | string | :material-checkbox-blank-circle: | `-` | The society name
| `Item`                | string | :material-checkbox-blank-circle: | `-` | The item name
| `Amount`                | number | :material-checkbox-blank-circle: | `-` | The amount

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    SocietyAddItem("police", "bread", 1)
    ```     

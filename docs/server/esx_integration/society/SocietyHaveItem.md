# SocietyHaveItem
Check if the society inventory have that item

| Argument              | Data Type                            | Needed                    | Default                       | Description
| ----------------------| ------------------------------------ | ------------------------- |-------------------------------|-------------
| `Society`                | string | :material-checkbox-blank-circle: | `-` | The society name
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
    local have_item = SocietyHaveItem("police", "bread")
    ```
# RemoveMoney
Remove money from the player

| Argument              | Data Type                            | Needed                    | Default                       | Description
| ----------------------| ------------------------------------ | ------------------------- |-------------------------------|-------------
| `id`                | number | :material-checkbox-blank-circle: | `-` |
| `Type`                | string | :material-checkbox-blank-circle: | `-` | The money type: cash, bank, black_money
| `Amount`                | number | :material-checkbox-blank-circle: | `-` | The amount of money

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    RemoveMoney(source, "cash", 500)
    
    RemoveMoney(source, "bank", 500)

    RemoveMoney(source, "black_money", 500)
    ```     

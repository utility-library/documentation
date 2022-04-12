# RemoveMoney
Remove money from the player

| Argument              | Data Type                            | Needed                    | Default                       | Description
| ----------------------| ------------------------------------ | ------------------------- |-------------------------------|-------------
| `Type`                | string | :material-checkbox-blank-circle: | `-` | The money type: cash, bank, black_money
| `Amount`                | number | :material-checkbox-blank-circle: | `-` | The amount of money

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    RemoveMoney("cash", 500)
    
    RemoveMoney("bank", 500)

    RemoveMoney("black_money", 500)
    ```     

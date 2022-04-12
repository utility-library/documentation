# AddMoney
Add money to the player

| Argument              | Data Type                            | Needed                    | Default                       | Description
| ----------------------| ------------------------------------ | ------------------------- |-------------------------------|-------------
| `Type`                | string | :material-checkbox-blank-circle: | `-` | The money type: cash, bank, black_money
| `Amount`                | number | :material-checkbox-blank-circle: | `-` | The amount of money

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    AddMoney("cash", 500)
    
    AddMoney("bank", 500)

    AddMoney("black_money", 500)
    ```     

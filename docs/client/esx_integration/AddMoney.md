# AddMoney (Client side)
Add money to the player

| Argument              | Data Type                            | Nedeed                    | Default                       | Description
| ----------------------| ------------------------------------ | ------------------------- |-------------------------------|-------------
| `Type`                | string | :material-checkbox-blank-circle: | `-` | The money type: cash, bank, black_money
| `Amount`                | number | :material-checkbox-blank-circle: | `-` | The amount of money

???+ warning
    For server safety, the trigger below the function can be disabled in the utility config

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    AddMoney("cash", 500)
    
    AddMoney("bank", 500)

    AddMoney("black_money", 500)
    ```     

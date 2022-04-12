# HaveMoney
Check if the player have that money

| Argument              | Data Type                            | Needed                    | Default                       | Description
| ----------------------| ------------------------------------ | ------------------------- |-------------------------------|-------------
| `Type`                | string | :material-checkbox-blank-circle: | `-` | The money type: cash, bank, black_money
| `Amount`                | number | :material-checkbox-blank-circle: | `-` | The amount of money to check

!!! success ""
    Dont need to be called every frame

??? success "Returns"
    | Data Type | Description                           |
    |-----------|---------------------------------------|
    | boolean   | If have or no the money                           |


---
??? example
    ```
    local have_money = HaveMoney("cash", 500)
    ```
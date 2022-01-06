# SocietyHaveMoney
Check if the society account have that money

| Argument              | Data Type                            | Nedeed                    | Default                       | Description
| ----------------------| ------------------------------------ | ------------------------- |-------------------------------|-------------
| `Society`                | string | :material-checkbox-blank-circle: | `-` | The society name
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
    local have_money = SocietyHaveMoney("police", 500)
    ```
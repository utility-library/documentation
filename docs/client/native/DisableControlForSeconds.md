# DisableCotrolForSeconds
Disable a key for inserted seconds

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Control`                | string | :material-checkbox-blank-circle: | `-` | The key to disable
| `Seconds`                | number | :material-checkbox-blank-circle: | `-` | The seconds which the button is disabled

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    DisableCotrolForSeconds("K", 5)
    ```
# InTimeRange
Checks if the time is within the specified time range (24h format)

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Min`                | number | :material-checkbox-blank-circle: | `-` | The minimum time in hour
| `Max`                | number | :material-checkbox-blank-circle: | `-` | The maximum time in hour
| `UTC`                | number | :material-checkbox-blank-circle-outline: | `false` | If this is true, use the UTC time to check the range

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    if InTimeRange(15, 18) then
        print("It's between 15 and 18")
    end
    ```
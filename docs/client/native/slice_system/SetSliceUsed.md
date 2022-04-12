# SetSliceUsed
Set a slice id as used

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `slice id`                | number | :material-checkbox-blank-circle: | `-` | The slice id 
| `used`                | boolean | :material-checkbox-blank-circle: | `-` | If is used or no

---
??? example
    ```
    local currentSlice = GetSelfSlice()
    SetSliceUsed(currentSlice, true)

    print("The current slice is used? "..SliceUsed(currentSlice)) -- The current slice is used? true
    ```
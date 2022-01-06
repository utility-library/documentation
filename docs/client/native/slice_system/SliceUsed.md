# SliceUsed
Check if a slice id is used

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `slice id`                | number | :material-checkbox-blank-circle: | `-` | The slice id


??? success "Returns"
    | Data Type                            | Description
    | ------------------------------------ |-------------
    | boolean | If is used or no

---
??? example
    ```
    print("There is something in my current slice? "..SliceUsed(GetCurrentSlice()))
    ```
# IsOnScreen
Check if some coords is in the screen

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `coords`                | vector3 | :material-checkbox-blank-circle: | `-` | The coords that whe need to check


??? success "Returns"
    | Data Type                            | Description
    | ------------------------------------ |-------------
    | boolean | If is on the screen

---
??? example
    ```
    print("The coords vector3(0.0, 0.0, 0.0) is on screen? "..IsOnScreen(vector3(0.0, 0.0, 0.0)))
    ```
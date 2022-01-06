# IsEntityFrozen
Check if the entity is frozen

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `entity`                | entity | :material-checkbox-blank-circle-outline: | `-` | The entity to check

??? success "Returns"
    | Data Type                            | Description
    | ------------------------------------ |-------------
    | boolean | True if is frozen, false if not
    
!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    IsEntityFrozen(entity)
    ```
# GetEntitySurfaceMaterial
Returns the hash of the ground material where the entity is in

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Entity`                | entity | :material-checkbox-blank-circle: | `-` | The entity being checked

??? success "Returns"
    | Data Type                            | Description
    | ------------------------------------ |-------------
    | materialHash | The material hash of the ground

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    local materialHash = GetEntitySurfaceMaterial(entity)
    ```
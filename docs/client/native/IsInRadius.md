# IsInRadius
Check the distance between 2 coords and return true if is in radius

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Coords 1`                | vector3 | :material-checkbox-blank-circle: | `-` | The first coords (probably the entity coords)
| `Coords 2`                | vector3 | :material-checkbox-blank-circle: | `-` | The second coords
| `Radius`                | number | :material-checkbox-blank-circle: | `-` | The distance to check
| `Sphere`                | boolean | :material-checkbox-blank-circle-outline: | `false` | Draw a sphere of the radius

??? success "Returns"
    | Data Type                            | Description
    | ------------------------------------ |-------------
    | boolean | If is in the radius

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    local near = IsInRadius(GetEntityCoords(entity), vector3(0.0,0.0,0.0), 10.0)
    ```
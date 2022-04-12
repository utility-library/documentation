# IsNearCoords
Check if the player is near to a coords

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Coords`                | vector3 | :material-checkbox-blank-circle: | `-` | The coords
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
    local near = IsNearCoords(vector3(0.0,0.0,0.0), 10.0)
    ```
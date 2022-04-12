# CreateCamera

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Coords`                | vector3 | :material-checkbox-blank-circle: | `-` | The coords to create the camera
| `Rotation`                | vector3 | :material-checkbox-blank-circle: | `-` | The rotation to create the camera
| `Active`                | boolean | :material-checkbox-blank-circle-outline: | `-` | If true switch on that cam
| `Shake`                | table | :material-checkbox-blank-circle-outline: | `-` | Shake or no

??? success "Returns"
    | Data Type                            | Description
    | ------------------------------------ |-------------
    | cam | The camera handle

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    local cam = CreateCamera(vector3(0.0, 0.0, 0.0), vector3(0.0, 0.0, 0.0), false, {type = "ROAD_VIBRATION_SHAKE", amount = 1.0})
    ```
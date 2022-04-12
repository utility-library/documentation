# DrawText3Ds
Draws 3D text on the specified coords

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Coords`                | vector3 | :material-checkbox-blank-circle: | `-` | The coordinates to create the 3d text
| `Text`                | string | :material-checkbox-blank-circle: | `-` | The text
| `Scale`                | number | :material-checkbox-blank-circle-outline: | `0.35` | The scale of the text
| `Font`                | number | :material-checkbox-blank-circle-outline: | `4` | The font, on the fivem native reference there isnt a list

!!! danger ""
    Need to be called every frame
---
??? example
    ```
    DrawText3Ds(vector3(0.0, 0.0, 0.0), "Test")
    ```
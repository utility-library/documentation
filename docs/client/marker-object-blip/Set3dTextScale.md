# Set3dTextScale
Set the scale of a marker (only 3d text)

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Id`                | string/number | :material-checkbox-blank-circle: | `-` | The id to update the marker
| `Scale`                | number | :material-checkbox-blank-circle: | `-` | The scale of the 3dtext
    
!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    Set3dTextScale("marker", 0.35)
    ```
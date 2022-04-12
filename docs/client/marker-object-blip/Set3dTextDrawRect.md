# Set3dTextDrawRect
Toggle if draw the black rectangle behind the text

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Id`                | string/number | :material-checkbox-blank-circle: | `-` | The id to update the marker
| `Active`                | boolean | :material-checkbox-blank-circle: | `-` | Active or not the black rectangle
    
!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    Set3dTextDrawRect("marker", true)
    ```
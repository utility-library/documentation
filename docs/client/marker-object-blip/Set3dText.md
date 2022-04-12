# Set3dText
Set the text of a 3d text

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Id`                | string/number | :material-checkbox-blank-circle: | `-` | The id to update the marker
| `Text`                | string | :material-checkbox-blank-circle: | `-` | The text to show
    
!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    Set3dText("marker", "Press [E] to interact")
    ```
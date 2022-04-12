# Set3dTextFont
Toggle if draw the black rectangle behind the text

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Id`                | string/number | :material-checkbox-blank-circle: | `-` | The id to update the marker
| `Font`                | boolean | :material-checkbox-blank-circle: | `-` | The [font id](https://gtaforums.com/topic/794014-fonts-list/)
    
!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    Set3dTextFont("marker", 4)
    ```
# SetMarker
Is the raw api that other api like `SetMarker` use. This is a more technic api that has not been thought to be used by anyone, if you don't have any idea of what this api can be, use the other already existing ones to set the data of the marker.

| Argument              | Data type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Id`                | string/number | :material-checkbox-blank-circle: | `-` | The id to update the marker
| `Data Type`                | string | :material-checkbox-blank-circle: | `-` | The type of the data inserted
| `Key`                | string | :material-checkbox-blank-circle: | `-` | The marker key to change
| `Value`                | any | :material-checkbox-blank-circle: | `-` | The marker new value
    
!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    SetMarker("marker", "string", "text", "Press [E] to interact")
    ```

??? info "Keys"
        | Key     | Data Type | Explanation |
        |-----------|-----------|------------ |
        | render_distance      | number    | The distance to render the marker                             |
        | interaction_distance      | number    | The distance where the interaction is enabled                       |
        | coords     | vector3    | The coords of the marker                            |
        | slice    | number    | The slice id of the marker |
        | rgb    | table   | The rgb color of the marker |
        | _type      | number   | The number of the marker (0 = 3d Text, 1 = Normal Marker)      |
        | text | string   | The text of the 3d text, if is a 3d text |
        | _direction | vector3 | The direction of the marker |
        | _rot | vector3 | The rotation of the marker |
        | _scale | vector3 | The scale of the marker |
        | alpha | number | The alpha of the marker (0-255) |
        | anim | boolean | Toggle the bouncing animation |
        | notify | string | The ButtonNotification text already converted to the GTA button style |
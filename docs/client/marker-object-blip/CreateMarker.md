# CreateMarker
Create a marker, can be an 3d text or real actual marker

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Id`                | string/number | :material-checkbox-blank-circle: | `-` | The id to manage the marker
| `Coords`                | vector3 | :material-checkbox-blank-circle: | `-` | The coordinates to create the marker
| `Render Distance`                | number | :material-checkbox-blank-circle: | `-` | The distance for the render
| `Interaction Distance`                | number | :material-checkbox-blank-circle: | `-` | The distance for the interaction
| `Options`                | table/string | :material-checkbox-blank-circle: | `-` | See the config arguments
    
!!! success ""
    Dont need to be called every frame, if called every frame and the marker already exist, sleep the loop for 100 ms to prevent spam
---
??? example
    Creating **marker**
    ```
    CreateMarker("myid", vector3(-239.89, -989.42, 28.29), 5.0, 5.0, {255, 0, 0})
    ```
    <img src="https://i.postimg.cc/pdrhXRW6/image.png" alt="" width="40%" heigth="40%"/><br>
    ---
    Creating **3d text**
    ```
    CreateMarker("myid", vector3(-239.89, -989.42, 29.29), 5.0, 5.0, "Press [~g~E~w~] to interact")
    ```
    <img src="https://i.postimg.cc/SQfy5Hq2/image.png" alt="" width="40%" heigth="40%"/>
    ---
    Creating a custom **marker** using a config
    ```
    local config = {
        rgb = {0, 0, 255},
        type = 29,
        scale = vector3(2.0, 2.0, 3.0),
    }

    CreateMarker("myid", vector3(-239.89, -989.42, 28.29), 5.0, 5.0, config)
    ```
    <img src="https://i.postimg.cc/PxRc3Pjh/image.png" alt="" width="40%" heigth="40%"/>

    ???+ abstract "Config arguments"
        | Child     | Data Type | Explanation |
        |-----------|-----------|------------ |
        | rgb      | table    | The rgb data (`{255, 255, 255}`)                             |
        | type     | number    | The [marker type](https://docs.fivem.net/docs/game-references/markers/)                            |
        | direction    | vector3    | The direction of the marker |
        | rotation    | vector3   | The rotation of the marker |
        | scale      | vector3   | The scale of the marker      |
        | alpha | number   | The alpha of the marker, from 0 to 255 |
        | animation | boolean | Toggle the bouncing animation |

??? info "How to listen the interaction"
    For listen the interaction you need to use the emitter

    !!! example
        ```
        -- This create the red marker
        CreateMarker("myid", vector3(-239.89, -989.42, 28.29), 5.0, 5.0, {255, 0, 0})
    
        -- Listening the interaction
        On("marker", function(id)
            if id == "myid" then
                print("Hello")
            end
        end)
        ```
        LSS: If i press E near the marker in the F8 console will be printed `Hello`

---
??? tip
    You can write `{r}` to generate a random id<br>

    !!! example
        ```
        CreateMarker("marker_{r}", vector3(-239.89, -989.42, 28.29), 5.0, 5.0, {255, 0, 0})
        ```
        This will be converted to "marker_51243", the number is the random id generated
??? danger "To do"
    :material-circle-slice-6: Adding more customization

*[LSS]: Long Story Short
*[idk]: I dont know
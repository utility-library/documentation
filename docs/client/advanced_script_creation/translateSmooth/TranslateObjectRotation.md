# TranslateObjectRotation
Rotate an entity with a constant speed.

| Argument        | Data Type | Needed                           | Default | Description                                                                                                                |
|-----------------|-----------|----------------------------------|---------|----------------------------------------------------------------------------------------------------------------------------|
| `obj`           | object    | :material-checkbox-blank-circle: | `-`     |                                                                                                                            |
| `destination`   | vector3   | :material-checkbox-blank-circle: | `-`     | The destination rotation                                                                                                   |
| `duration`      | number    | :material-checkbox-blank-circle: | `-`     | Total duration in ms                                                                                                       |
| `rotationOrder` | number    | :material-checkbox-blank-circle: | `-`     | The order yaw, pitch and roll is applied. Usually 2. Read more [here](https://docs.fivem.net/natives/?_0xAFBD61CC738D9EB9) |

!!! success ""
    Dont need to be called every frame

---
??? example
    ```
    local rot = GetEntityRotation(obj, 2)

    TranslateObjectRotation(obj, rot + vec3(0.0, 0.0, 90.0), 5000, 2)
    ```
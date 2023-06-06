# TranslateObjectCoords
Moves an entity with a constant speed.

| Argument      | Data Type | Needed                           | Default | Description          |
|---------------|-----------|----------------------------------|---------|----------------------|
| `obj`         | object    | :material-checkbox-blank-circle: | `-`     |                      |
| `destination` | vector3   | :material-checkbox-blank-circle: | `-`     | The destination coords, you can also use [GetOffsetFromEntityInWorldCoords](https://docs.fivem.net/natives/?_0x1899F328B0E12848)  |
| `duration`    | number    | :material-checkbox-blank-circle: | `-`     | Total duration in ms |

!!! success ""
    Dont need to be called every frame

---
??? example
    ```
    local offset = GetOffsetFromEntityInWorldCoords(obj, 2.0, 0.0, 0.0)

    TranslateObjectCoords(obj, offset, 5000)
    ```
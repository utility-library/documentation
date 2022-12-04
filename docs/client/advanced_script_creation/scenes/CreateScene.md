<<<<<<< HEAD
# CreateScene
Create a networked scene


| Argument        | Data Type | Needed                                   | Default | Description |
|-----------------|-----------|------------------------------------------|---------|-------------|
| `coords`        | vector3   | :material-checkbox-blank-circle:         | `-`     |             |
| `rot`           | vector3   | :material-checkbox-blank-circle:         | `-`     |             |
| `holdLastFrame` | boolean   | :material-checkbox-blank-circle-outline: | `false` |             |
| `looped`        | boolean   | :material-checkbox-blank-circle-outline: | `false` |             |
| `animSpeed`     | number    | :material-checkbox-blank-circle-outline: | `1.3`   |             |

??? success "Returns"
    | Data Type                            | Description
    | ------------------------------------ |-------------
    | scene | The scene netid

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    local player = PlayerPedId()
    local coords = GetEntityCoords(player)
    local rot = GetEntityRotation(player)

    local scene = CreateScene(coords, rot)
=======
# CreateScene
Create a networked scene


| Argument        | Data Type | Needed                                   | Default | Description |
|-----------------|-----------|------------------------------------------|---------|-------------|
| `coords`        | vector3   | :material-checkbox-blank-circle:         | `-`     |             |
| `rot`           | vector3   | :material-checkbox-blank-circle:         | `-`     |             |
| `holdLastFrame` | boolean   | :material-checkbox-blank-circle-outline: | `false` |             |
| `looped`        | boolean   | :material-checkbox-blank-circle-outline: | `false` |             |
| `animSpeed`     | number    | :material-checkbox-blank-circle-outline: | `1.3`   |             |

??? success "Returns"
    | Data Type                            | Description
    | ------------------------------------ |-------------
    | scene | The scene netid

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    local player = PlayerPedId()
    local coords = GetEntityCoords(player)
    local rot = GetEntityRotation(player)

    local scene = CreateScene(coords, rot)
>>>>>>> 2a78759c92d8c3cfcceba1661317ce3c33c6f503
    ```
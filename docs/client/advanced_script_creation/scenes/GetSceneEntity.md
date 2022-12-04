<<<<<<< HEAD
# GetSceneEntity
Return the entity with a specific model (only entity created by the scene)

| Argument   | Data Type     | Needed                                   | Default                                 | Description                                                       |
|------------|---------------|------------------------------------------|-----------------------------------------|-------------------------------------------------------------------|
| `scene`    | scene         | :material-checkbox-blank-circle:         | `-`                                     | The scene netid                                                   |
| `model`    | string/number | :material-checkbox-blank-circle:         | `-`                                     |                                                                   |

??? success "Returns"
    | Data Type                            | Description
    | ------------------------------------ |-------------
    | obj | The scene object

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    local entity = GetSceneEntity(scene, "prop_weed_01")
=======
# GetSceneEntity
Return the entity with a specific model (only entity created by the scene)

| Argument   | Data Type     | Needed                                   | Default                                 | Description                                                       |
|------------|---------------|------------------------------------------|-----------------------------------------|-------------------------------------------------------------------|
| `scene`    | scene         | :material-checkbox-blank-circle:         | `-`                                     | The scene netid                                                   |
| `model`    | string/number | :material-checkbox-blank-circle:         | `-`                                     |                                                                   |

??? success "Returns"
    | Data Type                            | Description
    | ------------------------------------ |-------------
    | obj | The scene object

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    local entity = GetSceneEntity(scene, "prop_weed_01")
>>>>>>> 2a78759c92d8c3cfcceba1661317ce3c33c6f503
    ```
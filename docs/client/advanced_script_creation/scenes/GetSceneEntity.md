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
    ```
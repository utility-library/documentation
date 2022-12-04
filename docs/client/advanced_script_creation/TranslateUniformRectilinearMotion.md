<<<<<<< HEAD
# TranslateUniformRectilinearMotion
Moves an entity in a uniform rectilinear motion up to three planes.
synchronizes with NetworkTime, so it can be called from the server by a client and it will be synchronized, it's a bit "advanced" logic to explain in a few words

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `obj`                | object | :material-checkbox-blank-circle: | `-` |
| `destination`                | number | :material-checkbox-blank-circle: | `-` |
| `duration`                | number | :material-checkbox-blank-circle: | `-` | Total duration in ms

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    local offset = GetOffsetFromEntityInWorldCoords(obj, 1.0, 1.0, 1.0)

    TranslateUniformRectilinearMotion(obj, offset, 5000) -- move the entity +1 in every plane
=======
# TranslateUniformRectilinearMotion
Moves an entity in a uniform rectilinear motion up to three planes.
synchronizes with NetworkTime, so it can be called from the server by a client and it will be synchronized, it's a bit "advanced" logic to explain in a few words

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `obj`                | object | :material-checkbox-blank-circle: | `-` |
| `destination`                | number | :material-checkbox-blank-circle: | `-` |
| `duration`                | number | :material-checkbox-blank-circle: | `-` | Total duration in ms

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    local offset = GetOffsetFromEntityInWorldCoords(obj, 1.0, 1.0, 1.0)

    TranslateUniformRectilinearMotion(obj, offset, 5000) -- move the entity +1 in every plane
>>>>>>> 2a78759c92d8c3cfcceba1661317ce3c33c6f503
    ```
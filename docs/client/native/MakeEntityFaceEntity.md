# MakeEntityFaceEntity
Makes the two entities look in the eye

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Entity 1`                | entity | :material-checkbox-blank-circle: | `-` | The first entity
| `Entity 2`                | entity | :material-checkbox-blank-circle: | `-` | The second entity
| `What entity`                | boolean | :material-checkbox-blank-circle-outline: | `false` | If true make the entity1 rotate to the entity2, otherwise the entity2 rotate to the entity1

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    MakeEntityFaceEntity(entity1, entity2)
    ```
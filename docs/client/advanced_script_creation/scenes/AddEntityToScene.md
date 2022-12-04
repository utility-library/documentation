<<<<<<< HEAD
# AddEntityToScene
Add an entity or create an entity and add it to an existing scene

| Argument          | Data Type     | Needed                                   | Default | Description                             |
|-------------------|---------------|------------------------------------------|---------|-----------------------------------------|
| `entity`          | string/object | :material-checkbox-blank-circle:         | `-`     | The entity or the model                 |
| `scene`           | scene         | :material-checkbox-blank-circle:         | `-`     | The scene netid                         |
| `dict`            | string        | :material-checkbox-blank-circle:         | `-`     | The anim dict that the entity will play |
| `name`            | string        | :material-checkbox-blank-circle:         | `-`     | The anim name that the entity will play |
| `speed`           | number        | :material-checkbox-blank-circle-outline: | `4.0`   |                                         |
| `speedMultiplier` | number        | :material-checkbox-blank-circle-outline: | `-8.0`  |                                         |
| `flag`            | number        | :material-checkbox-blank-circle-outline: | `1`     |                                         |

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    AddEntityToScene("prop_weed_01", scene, "somedict", "somename")
=======
# AddEntityToScene
Add an entity or create an entity and add it to an existing scene

| Argument          | Data Type     | Needed                                   | Default | Description                             |
|-------------------|---------------|------------------------------------------|---------|-----------------------------------------|
| `entity`          | string/object | :material-checkbox-blank-circle:         | `-`     | The entity or the model                 |
| `scene`           | scene         | :material-checkbox-blank-circle:         | `-`     | The scene netid                         |
| `dict`            | string        | :material-checkbox-blank-circle:         | `-`     | The anim dict that the entity will play |
| `name`            | string        | :material-checkbox-blank-circle:         | `-`     | The anim name that the entity will play |
| `speed`           | number        | :material-checkbox-blank-circle-outline: | `4.0`   |                                         |
| `speedMultiplier` | number        | :material-checkbox-blank-circle-outline: | `-8.0`  |                                         |
| `flag`            | number        | :material-checkbox-blank-circle-outline: | `1`     |                                         |

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    AddEntityToScene("prop_weed_01", scene, "somedict", "somename")
>>>>>>> 2a78759c92d8c3cfcceba1661317ce3c33c6f503
    ```
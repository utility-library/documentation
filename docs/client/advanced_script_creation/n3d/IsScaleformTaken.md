# IsScaleformTaken
Check if a default scaleform renderer (utility_lib_n) is taken from an n3d

| Argument                 | Data Type | Needed                           | Default | Description                  |
|--------------------------|-----------|----------------------------------|---------|------------------------------|
| `GFXName/Scaleform name` | string    | :material-checkbox-blank-circle: | `-`     | The name of your .gfx render |

!!! success ""
    Dont need to be called every frame

???+ success "Returns"
    | Child         | Data Type | Description |
    |---------------|-----------|-------------|
    | isTaken       | boolean   |             |

??? example
    ```
    local isTaken = IsScaleformTaken("utility_lib_9")
    ```
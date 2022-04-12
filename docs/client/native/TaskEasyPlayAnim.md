# TaskEasyPlayAnim
Simply asf the TaskPlayAnim, see argument below and compare it with the TaskPlayAnim

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Animation dictionary` | string | :material-checkbox-blank-circle: | `-` | The animation dictionary, [this is the list](https://alexguirre.github.io/animations-list/)
| `Animation name`       | string | :material-checkbox-blank-circle: | `-` | The animation name, [this is the list](https://alexguirre.github.io/animations-list/)
| `Flag`                 | number | :material-checkbox-blank-circle: | `51` | The animation flag: -1 loop, 51 moving, 0/50 stuck
| `Duration`             | number | :material-checkbox-blank-circle-outline: | `-1 (Infinite)` | The duration time in milliseconds (**ms**)

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    TaskEasyPlayAnim("amb@world_human_golf_player@male@idle_a", "idle_a")
    ```
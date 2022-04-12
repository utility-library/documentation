# SwitchBetweenCam

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Old Cam`                | cam | :material-checkbox-blank-circle: | `-` | The old cam
| `New Cam`                | cam | :material-checkbox-blank-circle: | `-` | The new cam
| `Duration`                | number | :material-checkbox-blank-circle-outline: | `1500` | The duration of the fade

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    SwitchBetweenCam(old_cam, cam)
    ```
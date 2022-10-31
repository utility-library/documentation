# CreateMissionText
Create a mission text at the bottom of the screen

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `msg`                | string | :material-checkbox-blank-circle: | `-` | The message to show
| `duration`                | number | :material-checkbox-blank-circle-outline: | `∞` | The duration of the mission text (ms)

??? success "Returns"
    | Data Type                            | Description
    | ------------------------------------ |-------------
    | table | A table with the delete method to clear the mission text

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    local mission = CreateMissionText("Hello World", 5000)
    Citizen.Wait(5000)
    mission:delete()
    ```
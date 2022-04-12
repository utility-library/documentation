# DeleteiObject
Delete a iObject

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Id`                | string/number | :material-checkbox-blank-circle: | `-` | The id of the iObject
| `Delete`            | boolean | :material-checkbox-blank-circle-outline: | `false` | If is true delete the actual entity, otherwise delete only the interaction


!!! success ""
    Dont need to be called every frame, if called every frame and the iObject dont exist, sleep the loop for 100 ms to prevent spam
---
??? example
    ```
    DeleteiObject("myid", true)
    ```
*[iObject]: Interactable Object
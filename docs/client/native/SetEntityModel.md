# SetEntityModel
Change the model of a entity over the network (also with local entities)

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `entity`                | entity | :material-checkbox-blank-circle: | `-` | 
| `model`                | string/number | :material-checkbox-blank-circle: | `-` | The new model


!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    SetEntityModel(obj, "prop_weed_01")
    ```
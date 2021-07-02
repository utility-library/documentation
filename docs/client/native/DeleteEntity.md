# DeleteEntity
Is equal to the standard one but request the control of the entity to prevent any deletion bug and set the entity as mission entity, can accept a netId

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Entity`                | entity/netId | :material-checkbox-blank-circle: | `-` | The entity handle or the netId of the entity
| `IsNetwork`                | boolean | :material-checkbox-blank-circle-outline: | `false` | If is true the entity arguments become the netId and find and delete the entity by the netId

!!! success ""
    Dont need to be called every frame
---
??? example
    Using **entity handle**
    ```
    DeleteEntity(entity, false)
    ```
    Using **netId**
    ```
    DeleteEntity(netId, true)
    ```
??? abstract "Old method"
    ```
    SetEntityAsMissionEntity(entity)
    DeleteEntity(entity)
    ```
    ???+ bug "Old method problem"
        Sometimes the entity is not deleted because the entity was created by another client
    ??? info "Using old native"
        although i dont recommend it, you can use the old native via `old_DeleteEntity`
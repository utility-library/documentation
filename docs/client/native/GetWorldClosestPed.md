# GetWorldClosestPed
Return the closest ped, and the all founded ped

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Radius`                | number | :material-checkbox-blank-circle: | `-` | The radius that being checked

??? success "Returns"
    | Data Type                            | Description
    | ------------------------------------ |-------------
    | ped | The closest ped
    | table | All the founded ped

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    local closest, allped = GetWorldClosestPed(5.0)
    ```
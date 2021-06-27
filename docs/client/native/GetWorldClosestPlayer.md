# GetWorldClosestPlayer
Return the closest player, and the all founded player

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Radius`                | number | :material-checkbox-blank-circle: | `-` | The radius that being checked

??? success "Returns"
    | Data Type                            | Description
    | ------------------------------------ |-------------
    | player | The closest player
    | table | All the founded player

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    local closest, allplayer = GetWorldClosestPlayer(5.0)
    ```
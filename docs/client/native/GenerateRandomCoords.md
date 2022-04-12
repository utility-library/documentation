# GenerateRandomCoords
Generate a random coords around the base coords

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Coords`                | vector3 | :material-checkbox-blank-circle: | `-` | The coords
| `Radius`                | number | :material-checkbox-blank-circle: | `-` | The limit for the generation
| `Heading`                | boolean | :material-checkbox-blank-circle-outline: | `false` | If true return a second parameter that is a random generated heading

??? success "Returns"
    | Data Type                            | Description
    | ------------------------------------ |-------------
    | vector3 | The generated coords
    | heading | The generated heading (only if the heading argument is true)

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    local coords = GenerateRandomCoords(GetEntityCoords(PlayerPedId()), 10.0)
    ```
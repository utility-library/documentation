# CreateGuardRoute
Creates a guard route that can be assigned to a guard

| Argument          | Data Type               | Needed                                   | Default | Description                                                    |
|-------------------|-------------------------|------------------------------------------|---------|----------------------------------------------------------------|
| `name`            | string                  | :material-checkbox-blank-circle:         | `-`     | A name to identify the guard route                             |
| `positions`       | vector3/vector4 (array) | :material-checkbox-blank-circle:         | `-`     | An array with the guard positions (vec4 its also with heading) |
| `manualRouteLink` | function                | :material-checkbox-blank-circle-outline: | `-`     | See the example                                                |

!!! success ""
    Dont need to be called every frame
---
??? example
    ```lua
    -- The guard will take this route in circular order (A > B > C > A)

    CreateGuardRoute("test", {
        vector3(1.0, 1.0, 1.0), -- A
        vector3(2.0, 2.0, 2.0), -- B
        vector3(3.0, 3.0, 3.0), -- C
    })
    ```

    Manual route linking
    ```
    local positions = {
        vector3(1.0, 1.0, 1.0), -- A
        vector3(2.0, 2.0, 2.0), -- B
        vector3(3.0, 3.0, 3.0), -- C
    }

    CreateGuardRoute("test", positions, function(last, current)
        if current == #positions then -- if is the last route, link it to the first (circular)
            AddPatrolRouteLink(current, 1) -- close the circle (C > A)
        end

        if current > 1 then -- if we need to link it
            AddPatrolRouteLink(last, current) -- (A > B) (B > C)
        end
    end)
    ```
# GetScaleformsStatus
Returns the status of the default scaleforms/gfx renderer (if is taken from a n3d)

!!! success ""
    Dont need to be called every frame

???+ success "Returns"
    | Child         | Data Type | Description                           |
    |---------------|-----------|---------------------------------------|
    | activeList    | table     | {name = scaleformName, data = n3d} |
    | inactiveList  | table     | {name = scaleformName, data = {}}  |

??? example
    ```
    local active, inactive = GetScaleformsStatus()

    print(inactive[1]) -- print the first scaleform/gfx available  
    ```
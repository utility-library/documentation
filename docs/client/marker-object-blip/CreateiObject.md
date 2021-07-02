# CreateiObject
Create a iObject

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Id`                | string/number | :material-checkbox-blank-circle: | `-` | The id to manage the iObject
| `Model`                | string/number | :material-checkbox-blank-circle: | `-` | The mode of the iObject
| `Coords`                | vector3 | :material-checkbox-blank-circle: | `-` | The coordinates to create the iObject
| `Heading`                | number | :material-checkbox-blank-circle: | `-` | The heading to create the iObject
| `Interaction Distance`                | number | :material-checkbox-blank-circle: | `-` | The distance for the interaction
    
??? success "Returns"
    | Data Type                            | Description
    | ------------------------------------ |-------------
    | iObject | The object handle
    | vector3 | The object coords

!!! success ""
    Dont need to be called every frame, if called every frame and the iObject already exist, sleep the loop for 100 ms to prevent spam
---
??? example
    Creating **iObject**
    ```
    local iobj, coords = CreateiObject("myid", "prop_weed_01", vector3(-239.89, -989.42, 28.29), 0.0, 5.0)
    ```

??? info "How to listen the interaction"
    For listen the interaction you need to use the emitter

    !!! example
        ```
        -- This create the iObject
        local iobj, coords = CreateiObject("myid", "prop_weed_01", vector3(-239.89, -989.42, 28.29), 0.0, 5.0)
    
        -- Listening the interaction
        On("object", function(id)
            if id == "myid" then
                print("Hello")
            end
        end)
        ```
        LSS: If i press E near the iObject in the F8 console will be printed `Hello`
*[LSS]: Long Story Short
*[iObject]: Interactable Object
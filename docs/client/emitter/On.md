# On
Is the listener of the emitter

| Argument           | Data Type | Needed                                   | Default | Description                                                                            |
|--------------------|-----------|------------------------------------------|---------|----------------------------------------------------------------------------------------|
| `Type`             | string    | :material-checkbox-blank-circle:         | `-`     | The type of the emitter                                                                |
| `Callback`         | function  | :material-checkbox-blank-circle:         | `-`     | The function that will be executed when the event has been triggered                   |
| `Fake Triggerable` | boolean   | :material-checkbox-blank-circle-outline: | `false` | If that is true you can use the trigger **Utility:FakeTrigger** to trigger the emitter |

## Emitter Types
| Name    | Description                                       | Parameters     |
|---------|---------------------------------------------------|----------------|
| marker  | Triggered when the player interact with a marker  | id             |
| object  | Triggered when the player interact with a iobject | id             |
| spotted | Triggered when the player is spotted by a guard   | guard (entity) |
| entered | Triggered when the player enter a marker/object   | type, id       |
| leaved  | Triggered when the player leave a marker/object   | type, id       |

!!! success ""
    Dont need to be called every frame
---

??? example
    ```
    On("marker", function(id)
        if id == "potato" then
            print("I love potato")
        elseif id == "carrot" then
            print("I hate carrot")
        end
    end)
    ```

    ??? info "Example of the fake trigger"
        ```
        --                                    Type       Id
        TriggerEvent("Utility:FakeTrigger", "marker", "potato")
        ```
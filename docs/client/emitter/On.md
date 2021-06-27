# On
Is the listener of the emitter

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Type`                | string | :material-checkbox-blank-circle: | `-` | The type of the emitter
| `Callback`            | function | :material-checkbox-blank-circle: | `-` | The function that will be executed when the event has been triggered
| `Fake Triggerable`    | boolean | :material-checkbox-blank-circle-outline: | `false` | If that is true you can use the trigger **Utility:FakeTrigger** to trigger the emitter

!!! success ""
    Dont need to be called every frame
---

??? example
    ```
    On("marker", function(id)
        if id == "potato" then
            print("I love potato")
        elseif id == "carrot" then
            print("I hate carrot)
        end
    end)
    ```

    ??? info "Example of the fake trigger"
        ```
        --                                    Type       Id
        TriggerEvent("Utility:FakeTrigger", "marker", "potato")
        ```
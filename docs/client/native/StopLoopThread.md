# StopLoopThread
Stop the [loop thread](http://127.0.0.1:8000/md/client/2_native/LoopThread/) identified by the id inserted

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Id`                | string/number | :material-checkbox-blank-circle: | `-` | The id of the loop thread

!!! success ""
    Dont need to be called every frame
---
???+ warning
    It can be used only into `CreateLoop` function where you created the thread
??? example
    ```
    StopLoopThread("first_loop")
    ```
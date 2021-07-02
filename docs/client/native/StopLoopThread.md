# StopLoopThread
Stop the [loop thread](https://utility-library.github.io/client/native/LoopThread/) identified by the id inserted

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Handle`                | string/number | :material-checkbox-blank-circle: | `-` | The handle of the loop thread

!!! success ""
    Dont need to be called every frame
---
???+ warning
    It can be used only into `CreateLoop` function where you created the thread
??? example
    ```
    StopLoopThread(myloopthread)
    ```
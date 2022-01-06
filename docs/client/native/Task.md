# Task
It will create a thread in the loop with a default time, can be stopped by the `StopLoopThread` using the id returned. 

**Available Task**

| Name              | Velocity                          
| ----------------------| ------------------------------------
| `TaskBack`                | 5000 ms
| `TaskSlow`                | 1000 ms
| `TaskFast`                | 500 ms
| `TaskExtraFast`                | 5 ms

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `LoopId`                  | number | :material-checkbox-blank-circle: | `-` | The loop id
| `Id`                      | string/number | :material-checkbox-blank-circle: | `-` | The id to identify the thread
| `Function`                | function | :material-checkbox-blank-circle: | `-` | The code executed in the loop thread

??? success "Returns"
    | Data Type                            | Description
    | ------------------------------------ |-------------
    | number | The handle of the LoopThread

!!! success ""
    Dont need to be called every frame
---
???+ warning
    It can be used only into `CreateLoop` function
??? example
    ```
    CreateLoop(function(loopId)
        TaskBack(loopId, "main", function()
            print("Hello")
        end)
    end, 250)
    ```
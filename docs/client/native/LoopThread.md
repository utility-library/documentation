# LoopThread
It will create a thread in the loop, the code inserted into the function will be executed each time for the inserted time, it can be used for optimize code (See example)

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `LoopId`                | number | :material-checkbox-blank-circle: | `-` | The loop id
| `Id`                | string/number | :material-checkbox-blank-circle: | `-` | The id to identify the thread
| `Time`                | number | :material-checkbox-blank-circle: | `-` | The time express in millisenconds (**ms**) of the execution
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
    **How it can be used for optimization**:
    ```
    local Luck = 1

    CreateLoop(function(loopId)
        LoopThread(loopId, "main", 500, function()
            Luck = Luck + 1
        end)

        print(Luck)
    end, 250)
    ```
    ??? success "Expected Results"
        *The thread overlaps because the thread time is a multiple of the time loop (in that case 2 or 3)*

        1<br>
        1<br>

        2<br>
        2<br>
        2<br>

        3<br>
        3<br>

        4<br>
        4<br>

        5<br>
        5<br>
        5<br>
        ...etc


    **How it works**:
    ```
    CreateLoop(function(loopId)
        print("Start")
        LoopThread(loopId, "main", 1000, function()
            print("Loop Thread")
        end)
        print("End")
    end, 500)
    ```
    ??? success "Expected Results"
        *The thread overlaps because the thread time is a multiple of the time loop (in that case 2 or 3)*

        Start<br>
        End<br>

        Start<br>
        LoopThread<br>
        End<br>

        Start<br>
        End<br>
        
        Start<br>
        LoopThread<br>
        End

        
        Start<br>
        End<br>
        ...etc

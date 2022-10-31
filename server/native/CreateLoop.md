# CreateLoop
Create a while true do loop

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Function`                | function | :material-checkbox-blank-circle: | `-` | The code executed in the loop
| `Time`                | number | :material-checkbox-blank-circle-outline: | `5` | The time express in millisenconds (**ms**) of the execution

!!! success ""
    Dont need to be called every frame
---
??? example
    **Without time**:
    ```
    CreateLoop(function()
        print("Test")
    end)
    ```
    **With time**:
    ```
    CreateLoop(function()
        print("Test")
    end, 500)
    ```
??? abstract "Old method"
    ```
    Citizen.CreateThread(function()
        while true do
            print("Test")
            Citizen.Wait(5)
        end
    end)
    ```
    ???+ bug "Old problem"
        In the old method if you forgot to insert `Citizen.Wait(ms)` the **ALL** server will crash<br>I created it because i was sick of the thousands of times my server crashed, Thanks FiveM 😉

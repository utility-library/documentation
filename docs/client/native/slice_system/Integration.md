# Integration in other script
The slice system allows you to optimize the scripts that control the distances by dividing the map into slice that every slice have an id, to integrate this system you must obtain the coordinates of where you want to get the slice id and simply call the function GetSliceFromCoords, after that you must set the slice as used with SetSliceUsed, to do the check create a loop that every 5 seconds or so assigns to a variable the current slice and check if the player is in a used slice, the used slice are not shared between scripts, as soon as the player is in the slice just check the coordinates for each coordinate in that slice

??? example
    ```lua
    local something = {}

    function CreateSomething(coords)
        local slice = GetSliceFromCoords(coords)

        table.insert(something, {slice = slice})
        SetSliceUsed(slice, true)
    end

    CreateLoop(function()
        slice = GetSelfSlice()
    end, 5000)

    CreateLoop(function()
        if SliceUsed(slice) then
            for i=1, #something do
                if something[i].slice == slice then
                    -- Is near a something
                end
            end
        end
    end)
    ```
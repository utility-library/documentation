# SetTextOf
Change the text of a marker by the id

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Type`                | string | :material-checkbox-blank-circle: | `-` | The type of the id:<br><br> Marker, marker, m <br>`or`<br> Object, object, o
| `Id`                | string/number | :material-checkbox-blank-circle: | `-` | The id
| `Text`                | string/number | :material-checkbox-blank-circle: | `-` | The new text

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    SetTextOf("marker", "myid", "Press [~g~E~w~] to rechange the text")
    ```
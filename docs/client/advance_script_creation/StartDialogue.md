# StartDialogue
Start a dialogue with a entity

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Entity`                | entity | :material-checkbox-blank-circle: | `-` | The entity with which you want to start a dialogue
| `Distance`                | number | :material-checkbox-blank-circle: | `-` | The distance
| `Function`                | function | :material-checkbox-blank-circle: | `-` | The function that is called when the player responds with the entity

??? success "Returns"
    | Child     | Data Type | Description                           |
    |-----------|-----------|---------------------------------------|
    | Question      | function    | The function to set the questions
    | Response      | function    | The function to set the responses
    | LastQuestion      | function    | The function to set the last response by the entity

???+ warning
    You can start only `1` dialogue at time

!!! success ""
    Dont need to be called every frame
---
??? example
    <img src="https://i.postimg.cc/dtYsDk0c/immagine-2021-06-30-222252.png" alt="" width="80%" heigth="80%"/>
    <img src="https://i.postimg.cc/K8D0PVF8/image.png" alt="" width="40%" heigth="40%"/>

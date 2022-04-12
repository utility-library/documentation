# EditDialogue
Edit an already created dialogue with a entity

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Entity`                | string/number | :material-checkbox-blank-circle: | `-` | The entity that handle the dialogue

??? success "Returns"
    | Child     | Data Type | Description                           |
    |-----------|-----------|---------------------------------------|
    | Question      | function    | The function to set the questions
    | Response      | function    | The function to set the responses
    | LastQuestion      | function    | The function to set the last response by the entity

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    EditDialogue(entity)
    .Question({
        "Utility is the revolution"
    })
    .Response(
        {
            ["~g~[E]"] = "I totally agree with you"
        }
    )
    ```

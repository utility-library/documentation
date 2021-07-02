# EditDialogue
Edit an already created dialogue with a entity

??? success "Returns"
    | Child     | Data Type | Description                           |
    |-----------|-----------|---------------------------------------|
    | Question      | function    | The function to set the questions
    | Response      | function    | The function to set the responses
    | LastQuestion      | function    | The function to set the last response by the entity

???+ warning
    Can be used only in a `StartDialogue` function

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    EditDialogue()
    .Question({
        "Utility is the revolution"
    })
    .Response(
        {
            ["~g~[E]"] = "I totally agree with you"
        }
    )
    ```

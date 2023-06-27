```mermaid
sequenceDiagram
    participant browser
    participant server

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server

    server-->>browser: Confirmation to the browser that the note was created
    deactivate server

    Note right of the browser: The browser starts executing the JavaScript code that displays the new note on the page
```
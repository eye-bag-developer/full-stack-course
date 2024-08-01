sequenceDiagram
    participant browser
    participant server

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    server-->>browser: 201 new note created
    deactivate server

    Note right of browser: New note {content: "test spa", date: "2024-08-01T22:33:02.248Z"} created and added to notes
sequenceDiagram
    participant browser
    participant server

    Note right of browser: User types text into the input field and clicks Save

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/spa
    activate server
    Note right of server: Server processes the new note
    server-->>browser: updates notes list
    deactivate server


# Exercise 0.6


```mermaid
sequenceDiagram
    participant browser
    participant server

    Note right of browser: The browser executes the JavaScript code to create and send the new note as JSON data to the server

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    server-->>browser: 201 created
    deactivate server

    Note right of browser: The browser executes the callback function that renders the notes
````







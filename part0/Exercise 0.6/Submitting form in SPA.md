```mermaid
sequenceDiagram
    participant browser
    participant server

browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
activate server
server-->>browser: Status 201: Created

Note  right of browser: Content and Date in form is pushed by event handler and used by Javascript code to be added to notes
```

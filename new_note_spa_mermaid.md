```mermaid
sequenceDiagram
    participant browser
    participant server
 browser->>server: POST [https://studies.cs.helsinki.fi/exampleapp/new_note_spa]
 Note right of browser: add new note as JSON to notes array in data.json
 Note right of browser: prevent redirect - rerender page with new note contained in data.json in browser
 Note right of browser: create POST request to update data.json on server with new note
```

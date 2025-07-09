```mermaid
sequence diagram
  participant browser
  participant server

  browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/spa
Note right of browser: Only one request, and no redirect
  activate server
  server-->>browser: 201 Created
  deactivate server

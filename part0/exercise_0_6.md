```mermaid
sequenceDiagram
  participant browser
  participant server

  browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/spa
  activate server
Note right of browser: Only one request, and no redirect
  server-->>browser: 201 Created
  deactivate server
````

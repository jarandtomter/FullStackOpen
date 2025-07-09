```mermaid
sequenceDiagram
  participant browser
  participant server

  browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/spa
  activate server
Note right of browser: Only fetches one HTML
  server-->>browser: HTML with js

````

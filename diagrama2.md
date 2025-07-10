﻿```mermaid
deploymentDiagram
  artifact DispositivoM�vil {
    [APK Realidad Aumentada]
    [C�mara/Sensores]
    [ARCore/ARKit]
  }
  node Servidor {
    [API REST] --> [Base de Datos]
  }
  node P�ginaWeb {
    [Frontend]
    [HTML/CSS/JS]
  }
  DispositivoM�vil - HTTP/HTTPS -> Servidor
  Servidor - HTTP/HTTPS -> P�ginaWeb
  classDef mobile fill:#e3f2fd,stroke:#2196f3;
  classDef server fill:#ffebee,stroke:#f44336;
  classDef web fill:#e8f5e9,stroke:#4caf50;
  class DispositivoM�vil mobile;
  class Servidor server;
  class P�ginaWeb web;
```
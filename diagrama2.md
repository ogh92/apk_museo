```mermaid
deploymentDiagram
  artifact DispositivoMóvil {
    [APK Realidad Aumentada]
    [Cámara/Sensores]
    [ARCore/ARKit]
  }
  node Servidor {
    [API REST] --> [Base de Datos]
  }
  node PáginaWeb {
    [Frontend]
    [HTML/CSS/JS]
  }
  DispositivoMóvil - HTTP/HTTPS -> Servidor
  Servidor - HTTP/HTTPS -> PáginaWeb
  classDef mobile fill:#e3f2fd,stroke:#2196f3;
  classDef server fill:#ffebee,stroke:#f44336;
  classDef web fill:#e8f5e9,stroke:#4caf50;
  class DispositivoMóvil mobile;
  class Servidor server;
  class PáginaWeb web;
```
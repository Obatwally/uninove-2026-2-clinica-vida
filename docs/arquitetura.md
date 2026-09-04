```mermaid
sequenceDiagram
    participant N as Navegador do paciente
    participant D as Servidor DNS
    participant S as Servidor da Clínica Vida+
    N->>D: clinicavidamais.com.br?
    D-->>N: 203.0.113.42
    N->>S: conexão TCP e TLS na porta 443
    N->>S: GET /consultas/agendar
    S-->>N: 200 OK, HTML da agenda
```

## Evidência do DNS

```
186.251.39.123
```
| Recurso | Método | Status |
|---|---|---|
| www.uninove.br | GET | 200 |
| gtm.js | GET | 304 |
| index.497f13d13.css | GET | 200 |
| x-icon.png | GET | 200 |

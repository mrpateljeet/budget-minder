**Deployment Diagram**
```mermaid
graph TD
    A[User] -->|Browser| B[Frontend]
    B -->|HTTP Requests| C[Backend]
    C --> D[In-Memory Storage]

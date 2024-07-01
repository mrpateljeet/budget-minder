### Sequence Diagram
```mermaid
sequenceDiagram
    participant User
    participant Frontend
    participant Backend

    User ->> Frontend: Access Registration Form
    User ->> Frontend: Fill Form and Submit
    Frontend ->> Backend: Send Registration Data
    Backend ->> Backend: Hash Password and Store Data
    Backend ->> Frontend: Send Success Response
    Frontend ->> User: Show Success Message

    User ->> Frontend: Access Login Form
    User ->> Frontend: Fill Form and Submit
    Frontend ->> Backend: Send Login Data
    Backend ->> Backend: Verify Credentials
    Backend ->> Frontend: Send JWT Token
    Frontend ->> User: Show Success Message

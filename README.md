# Hello
```mermaid
  graph TD;
      A-->B;
      A-->C;
      B-->D;
      C-->D;
```
```mermaid
sequenceDiagram
    actor User
    actor Admin
    participant System
    participant Payment

    User ->> System: Book Movie
    User ->> System: Cancel Movie
    User ->> System: Book Events
    User ->> System: Cancel Events
    
    Admin ->> System: Update Information
    
    System ->> Payment: Process Payment
    Payment ->> User: Payment Options (Credit, Debit, Netbanking)
```
```mermaid
 sequenceDiagram
     actor Actor
 ```

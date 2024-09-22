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
```plantuml
@startuml
actor User
actor Admin

User -> (Book Movie)
User -> (Cancel Movie)
User -> (Book Events)
User -> (Cancel Events)

Admin -> (Update Information)

(Book Movie) --> (System)
(Cancel Movie) --> (System)
(Book Events) --> (System)
(Cancel Events) --> (System)
(Admin) --> (System)

(System) --> (Payment)

(Payment) --> (Credit)
(Payment) --> (Debit)
(Payment) --> (Netbanking)
@enduml
```

```mermaid
sequenceDiagram
    participant user
    participant system
    participant admin

    user->> system: book movie
    system-->> user: confirmation
    user->> system: cancel movie
    system-->> user: confirmation
    user->> system: book events
    system-->> user: confirmation
    user->> system: cancel events
    system-->> user: confirmation
    admin->> system: update information
    system-->> admin: confirmation
    system->> system: payment
    system->> system: credit
    system->> system: debit
    system->> system: netbanking
```

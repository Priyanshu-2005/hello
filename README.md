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

    User --> |Book Movie| BookMovie[Book Movie]
    User --> |Cancel Movie| CancelMovie[Cancel Movie]
    User --> |Book Events| BookEvents[Book Events]
    User --> |Cancel Events| CancelEvents[Cancel Events]

    Admin --> |Update Information| UpdateInfo[Update Information]

    BookMovie --> System((System))
    CancelMovie --> System
    BookEvents --> System
    CancelEvents --> System
    UpdateInfo --> System
    
    System --> Payment[Payment]
    
    Payment --> Credit[Credit]
    Payment --> Debit[Debit]
    Payment --> Netbanking[Netbanking]
```
```mermaid
 sequenceDiagram
     actor Actor
 ```

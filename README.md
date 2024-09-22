# Hello
```mermaid
  graph TD;
      A-->B;
      A-->C;
      B-->D;
      C-->D;
```
```sequenceDiagram
    actor Alice
    actor Bob
    Alice->>Bob: Hi Bob
    Bob->>Alice: Hi Alice
```


```sequenceDiagram
  graph TD
    actor user
    user --> A1[Book Movie]
    user --> A2[Cancel Movie]
    user --> A3[Book Events]
    user --> A4[Cancel Events]

  actor admin
    admin --> A5[Update Information]

  actor system
    A1 --> system
    A2 --> system
    A3 --> system
    A4 --> system
    A5 --> system
    
    system --> A6[Payment]
    
    A6 --> B1[Credit]
    A6 --> B2[Debit]
    A6 --> B3[Netbanking]


```

```graph TD
    User((User)) --> |Book Movie| BookMovie[Book Movie]
    User --> |Cancel Movie| CancelMovie[Cancel Movie]
    User --> |Book Events| BookEvents[Book Events]
    User --> |Cancel Events| CancelEvents[Cancel Events]

    Admin((Admin)) --> |Update Information| UpdateInfo[Update Information]

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

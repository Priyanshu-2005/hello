# Hello
```mermaid
  graph TD;
      A-->B;
      A-->C;
      B-->D;
      C-->D;
```

```mermaid
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

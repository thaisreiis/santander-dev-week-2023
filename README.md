# Santander Dev Week 2023
Java RESTful API criada para a Santander Dev Week

## Diagrama de Classes

```mermaid
classDiagram
  class User {
    -name: String
    -account: Account
    -feactures: Feacture[]
    -card: Card
    -news: News[]
  }

  class Account {
    -number: String
    -agency: String
    -balance: Number
    -limit: Number
  }

  class Feacture {
    -icon: String
    -description: String
  }

  class Card {
    -number: String
    -limit: Number
  }

  class News {
    -icon: String
    -description: String
  }

  User "1" *-- "1" Account
  User "1" *-- "N" Feacture
  User "1" *-- "1" Card
  User "1" *-- "N" News
```

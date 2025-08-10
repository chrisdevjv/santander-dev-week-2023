# Santander Dev Week 2023
Java RESTful API criada para a Santander Dev Week.

## Diagrama de Classes

```mermaid

classDiagram
    class User {
        +string name
    }

    class Account {
        +string number
        +string agency
        +float balance
        +float limit
    }

    class Feature {
        +string icon
        +string description
    }

    class Card {
        +string number
        +float limit
    }

    class News {
        +string icon
        +string description
    }

    User --> Account : account
    User --> "0..*" Feature : features
    User --> Card : card
    User --> "0..*" News : news
```

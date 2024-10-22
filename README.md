# Sistema de E-commerce

# Diagrama de Classe

```mermaid
classDiagram
    class Product {
        +Long id
        +String name
        +double price
        +int stockQuantity
    }
    
    class Customer {
        +Long id
        +String name
        +String email
        +String address
    }

    class Order {
        +Long id
        +String status
        +Customer customer
        +List~Product~ products
    }

    Product --* Order : contains
    Customer --* Order : places
```

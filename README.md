erDiagram
    CUSTOMER {
        int CustomerID
        string Name
        string Email
    }
    ORDER {
        int OrderID
        int CustomerID
        string OrderDate
    }
    PRODUCT {
        int ProductID
        string Name
        float Price
    }

    CUSTOMER ||--o{ ORDER : places
    ORDER ||--|{ PRODUCT : contains

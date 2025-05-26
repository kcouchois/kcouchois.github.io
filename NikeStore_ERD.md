```mermaid
erDiagram
    CUSTOMER }|..|{ PRODUCT : views
    CUSTOMER {
        string custname
        string custnumber
        string custaddress
    }
    PRODUCT {
        string prodtype
        string proddescription
        string prodnumber
    }
    ORDER-ITEM ||--|{ SALE : creates
    INVENTORY ||--o{ PRODUCT : contains
    INVENTORY {
        string inventorynumber
    }
    PRODUCT ||--o{ ORDER-ITEM : "ordered in"
```
#Brief Description
- Customers buy the products you supply
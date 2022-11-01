# Mermaid C4 Context Diagram

```mermaid
C4Context
    title C4 Context Diagram

    Person(customer, "Customer", "Online Customer")
    System(eCommerce, "E-Commerce", "E-Commerce System")
    System_Ext(stripe, "Stripe", "Payments")
    System_Ext(warehouse, "Warehouse", "Stock inventory and dispatch")

    Rel_D(customer, eCommerce, "orders products", "HTTPS")
    Rel_L(eCommerce, stripe, "process payment", "HTTPS")
    Rel_D(eCommerce, warehouse, "check stock", "HTTPS")
```

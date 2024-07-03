# Record availability of each line item in metafield on order create

Tags: Orders, Order Attributes, Line Items, Metafields

On order creation, this task will record the availability of each line item in the order. The record will show the SKU of the line item, as well as its availability, be it In Stock, Pre-Order, or ISPO (a combination of both). This is currently used in conjunction with the task **Tag orders in bulk depending on line item availability**.

## Subscriptions

```liquid
  shopify/orders/create
```

[Read Lightward's Mechanic event subscriptions documentation](https://learn.mechanic.dev/core/tasks/subscriptions)
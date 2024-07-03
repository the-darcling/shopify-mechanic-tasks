# Send a notification to customer of each line item availability one day later

Tags: Orders, Order Attributes, Line Items, Email

This task will send an email to the customer exactly one day after they've placed their order, containing the availability (Pre-Order, In Stock, ISPO) status of each of the line items in their order. It uses the order attributes set by the **Tag orders in bulk depending on line item availability** automation.

## Subscriptions

```liquid
  shopify/orders/create
  user/orders/availability
```

[Read Lightward's Mechanic event subscriptions documentation](https://learn.mechanic.dev/core/tasks/subscriptions)
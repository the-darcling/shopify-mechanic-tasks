# Tag orders in bulk depending on line item availability

Tags: Orders, Order Attributes, Line Items

Every midnight and midday, this task will automatically go through all unfulfilled and partially fulfilled orders, from oldest to newest, and determine if each order should be tagged In Stock, Pre-Order, or ISPO (a combination of both).

## Subscriptions

```liquid
  mechanic/user/trigger
  mechanic/scheduler/daily
  user/scheduler/midday
```

[Read Lightward's Mechanic event subscriptions documentation](https://learn.mechanic.dev/core/tasks/subscriptions)

### Personal note

One of the two tasks I'm very proud to have written; this task was one I had created specifically to help our warehouse manage the fulfillment of orders. The creation of this task rendered our warehouse's manual stock reservation system obsolete.

Explanation: we have product variants that are open for pre-order, and product variants that are in stock. Often, customers opt to check out with a mix of both pre-order and in stock variants. When this happens, warehouse needs to wait for all the products to come into stock before shipping out the entire order. Prior to this automation, warehouse was keeping track of the above manually, needing to make sure that the oldest orders were prioritised. There was lots of human error. So I pitched this automation to management and they were pleased ♡
# Tag orders in bulk depending on line item availability

Tags: Orders, Order Attributes, Line Items

Every midnight and midday, this task will automatically go through all unfulfilled and partially fulfilled orders, from oldest to newest, and determine if each order should be tagged In Stock, Pre-Order, or ISPO (a combination of both).

## Subscriptions

```liquid
  mechanic/user/trigger
  mechanic/scheduler/daily
  user/scheduler/midday
```

[Lightward's Mechanic event subscriptions documentation](https://learn.mechanic.dev/core/tasks/subscriptions)

## Documentation

Every midnight and midday, this task will automatically go through all unfulfilled and partially fulfilled orders, from oldest to newest, and determine if each order should be tagged In Stock, Pre-Order, or ISPO (a combination of both).

## Installing this task


Find this task in the library at tasks.mechanic.dev, and use the "Try this task" button. Or, import this task's JSON export – see Importing and exporting tasks to learn how imports work.

# Entity Relationship Map

## Core Entities

- User
- Expense
- Category
- Product
- ProductGroup
- Budget
- RecurringExpense
- Attachment

## Relationships

- Category 1:N Expense
- ProductGroup 1:N Product
- Product 1:N Expense (optional)
- User 1:N Expense
- Budget N:1 Category
- RecurringExpense N:1 Category

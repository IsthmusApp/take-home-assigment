# Isthmus backend take home assignment

Building under constraints, both of time and resources, is a reality of working in a startup. In this exercise, we’d like to understand your process to build an API from scratch, as well as how you choose to focus during a limited amount of time.

In this exercise, we’d like you to build out an api based on the specs below. We’d like you to time box this exercise to no more than 4 hours with the goal being to better understand your thinking and approach to spinning up a new application under a time constraint.

## Specs

We’d like you to demonstrate your backend knowledge by building a products inventory API.

The goal of this work is to see how you think via code and how you’d prioritize under a time constraint. Feel free to make whatever technical design decisions you need to make progress in this short amount of time.

Code quality and project decisions about gems, classes and tools used will be evaluated.

## Build a product inventory API

The goal of this assignment is to build a Ruby on Rails API (REST or GraphQL) that can create, update, delete, show and list products.

#### The structure of a product is the following:

```typescript
{
  id: string | number,
  name: string,
  description?: text,
  archived: boolean,
  price: number,
  quantity: number,
  categories: string[],
  created_at: datetime,
  updated_at: datetime,
}
```

### Create
I can create a new product by informing all of the required attributes.

### Update
I can update a product by informing it's ID and any attributes (except ID, created_at and updated_at).

### Delete
I can delete a product by informing it's ID.

### Show
I can show a product by informing it's ID.

### List
I can list all products and filter by the following attributes:

```typescript
{
  archived?: boolean,
  categories?: string[], // AND filter,
  price?: number // bigger than, lower than
}
```

Please add a README.md to the project explaining how to run and use it (REST endpoints or Graphql examples).

## Extra points

- GraphQL API
- Bulk update products
- Show history of product quantity changes over time
- Deploy it somewhere

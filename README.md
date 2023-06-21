# CoreGraphQL

## Description
This project is an example implementation of a GraphQL API using .NET Core. It demonstrates how to create and interact with a product management system.

## Features
- Create a new product
- Retrieve product information
- Update product details
- Delete a product

## Installation
1. Clone the repository: `git clone https://github.com/ebenvpaul/CoreGraphQL.git`
2. Navigate to the project directory: `cd CoreGraphQL`
3. Restore the dependencies: `dotnet restore`
## Usage
1. Start the application: `dotnet run`
2. Access the GraphQL UI using the following URL: [https://localhost:7287/ui/altair](https://localhost:7287/ui/altair)
3. Use the GraphQL UI to interact with the API and perform queries and mutations.

## GraphQL API
The GraphQL API is accessible at the endpoint: [https://localhost:7287/graphql](https://localhost:7287/graphql)

## Examples
1.Query Products
```query
{
  products {
    id
    name
    quantity
  }
}
```
2. Create a new product:
```graphql
mutation {
  createProduct(product: {
    name: "Sample Product",
    quantity: 10
  }) {
    id
    name
    quantity
  }
}
```
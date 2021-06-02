# Technical Evaluation - Senior Frontend Developer

Time allocated: 2 hours

## Scope

In this technical evaluation, you are expected to build a straightforward e-commerce application.

The application should consist of the following:

### Product Listing: `/products`

- View all available products, with pagination
- Search for a product
- Filter by:
  - Product category
  - Brand

### Product detail: `/products/:productId`

- View product information
- Images
- Product reviews
- Price information
- Product attributes (color, etc)
- Add to cart

### Bonus

- Basic Cart implementation
- Jest or Cypress

## Requirements

- Must be built in React. Specific Framework is your choice.
- SEO Friendly.
- No need to worry about mobile here, that’s not what we’re evaluating.

## Provided Data

### Algolia

We use Algolia, a search indexing platform, for building stores. This particular index contains the products used for this exercise. The index name is `dev_PRODUCTS`. You will be provided with an API key, and the Application ID required for the integration.

The documentation for Algolia can be found [here](https://www.algolia.com/doc/api-reference/widgets/react/).

### Endpoints for retrieving product information

We have provided two endpoints for returning information on products. These will be given to you at the start of the exercise.

#### `/:productId/metadata` 

**Example response:**

```ts
{
  objectId: String,
  name: String,
  images: [String],
  brand: String,
  categories: [String],
  attributes: {
    case_size: String,
    wristband_size: String,
    color: String
  },
  description: String,
  reviews: [
    {
      name: String,
      content: String,
      rating: Number
    }
  ]
}
```

#### `/:productId/price`

**Example response:**

```ts
{
  objectId: String,
  amount: String,
  currency: String
}
```

**Good luck!**

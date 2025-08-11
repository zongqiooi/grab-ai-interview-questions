# Concedo: AI-Centric Interview Process

## Exercise 2: Backend API Design and Optimisation

**Task**

"You need to create a backend server that serves product data via an API endpoint.You may use your AI assistant."

**Getting Started**

*   You can use **Node.js/Express**, **Django**, **Flask**, or any backend framework of your choice.
*   Use your preferred AI assistant (GitHub Copilot, ChatGPT, Claude, Cursor, etc.) to collaboratively design and develop the solution

**Your Challenge**

Create a backend server with the following functionality:

*   Set up a **localhost server** with an endpoint **/api/products** to serve the provided JSON data.
*   Use the JSON data format provided in the **data.json** file.

1.  Get Data Endpoint with a filtering option:

*   Add query parameters to the **/api/products** endpoint to filter products based on:
    *   **Price** (price <= 100)
    *   **Average review rating** (rating >= 3)

1.  Suggestion Endpoint:

*   Implement another endpoint **/api/suggestions** that accepts a customer’s budget as a query parameter and returns combinations of two products whose prices are equal to or below the budget. \*Ignore the discount, use the price as is.
    *   Example input: **budget = 10**
    *   Example output:

```json
{
  "suggestions": [
    [
      "product_a_name",
      "product_b_name"
    ],
    [
      "product_c_name",
      "product_d_name"
    ],
    ... 
  ]
}
Error Handling:
Handle cases where the request is invalid, or no data matches the filters or budget constraints. For example, query params for only price and rating.
Code Quality:
Follow good coding practices with clear file and code structure.
Ensure the code is modular and easy to maintain.
JSON Data Format

Use the following JSON data format for the task:
{
  "products": [
    {
      "id": 1,
      "title": "Essence Mascara Lash Princess",
      "description": "The Essence Mascara Lash Princess is a popular mascara known for its volumizing and lengthening effects. Achieve dramatic lashes with this long-lasting and cruelty-free formula.",
      "category": "beauty",
      "price": 9.99,
      "rating": 2.56
    },
    {
      "id": 2,
      "title": "Eyeshadow Palette with Mirror",
      "description": "The Eyeshadow Palette with Mirror offers a versatile range of eyeshadow shades for creating stunning eye looks. With a built-in mirror, it's convenient for on-the-go makeup application.",
      "category": "beauty",
      "price": 19.99,
      "rating": 2.86
    }
    ...
  ],
  "total": 194
}
```

**Success Criteria** \n
✅ Successfully set up a backend server with endpoints to serve product data \n
✅ Handle filtering and suggestion logic efficiently \n
✅ Implement error handling for invalid requests or empty results \n
✅ Optimise code structure and readability \n
✅ Follow good coding practices \n\n

Good luck! Remember, we're interested in your process as much as your final solution.

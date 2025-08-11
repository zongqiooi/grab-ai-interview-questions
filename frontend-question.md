# Concedo: AI-Centric Interview Process

## Exercise 1: Frontend Table with API Integration and Optimisation

**Task**

"You need to create a frontend table that displays product data fetched from an API. Use your AI assistant to help you implement and optimize this feature."

**Getting Started**

*   You can use **React/Angular/Next/Vanilla JS** or any frameworks for the frontend.
*   Use your preferred AI assistant (GitHub Copilot, ChatGPT, Claude, Cursor, etc.) to collaboratively code the solution.

**Your Challenge**

Create a page with the following functionality:

*   **Fetch product data**:
    *   Use the API endpoint:
        *   Sample: <https://dummyjson.com/products>
        *   API Docs: <https://dummyjson.com/docs/products>
    *   No API key is required for this free testing API.
*   **Display all the data in a table**:
    *   Include product details such as **title**, **description**, **price**, and **category**.
*   **Styling**:
    *   Improve the table's UI/UX for better readability and user experience.
*   **Additional Logic**:
    *   Add a new column, “**average\_review”,** to display the average score of the reviews of each product.
        *   This is to be derived from the “**reviews**” column data.
    *   Implement a **frontend** search feature based on **title**.
*   **Proper Error Handling**:
    *   Handle cases where the API request fails or returns invalid data.

**API Information**

**Endpoint**: <https://dummyjson.com/products>

**API Docs**: <https://dummyjson.com/docs/products>

**Method**: GET

**Expected Response Format**:

```json
{
  "products": [
    {
      "id": 1,
      "title": "Essence Mascara Lash Princess",
      "description": "The Essence Mascara Lash Princess is a popular mascara known for its volumizing and lengthening effects. Achieve dramatic lashes with this long-lasting and cruelty-free formula.",
      "category": "beauty",
      "price": 9.99,
      "discountPercentage": 10.48,
      "rating": 2.56,
      "stock": 99,
      "tags": [
        "beauty",
        "mascara"
      ],
      "brand": "Essence",
      "sku": "BEA-ESS-ESS-001",
      "weight": 4,
      "dimensions": {
        "width": 15.14,
        "height": 13.08,
        "depth": 22.99
      },
      "warrantyInformation": "1 week warranty",
      "shippingInformation": "Ships in 3-5 business days",
      "availabilityStatus": "In Stock",
      "reviews": [
        {
          "rating": 3,
          "comment": "Would not recommend!",
          "date": "2025-04-30T09:41:02.053Z",
          "reviewerName": "Eleanor Collins",
          "reviewerEmail": "eleanor.collins@x.dummyjson.com"
        },
        {
          "rating": 4,
          "comment": "Very satisfied!",
          "date": "2025-04-30T09:41:02.053Z",
          "reviewerName": "Lucas Gordon",
          "reviewerEmail": "lucas.gordon@x.dummyjson.com"
        },
        {
          "rating": 5,
          "comment": "Highly impressed!",
          "date": "2025-04-30T09:41:02.053Z",
          "reviewerName": "Eleanor Collins",
          "reviewerEmail": "eleanor.collins@x.dummyjson.com"
        }
      ],
      "returnPolicy": "No return policy",
      "minimumOrderQuantity": 48,
      "meta": {
        "createdAt": "2025-04-30T09:41:02.053Z",
        "updatedAt": "2025-04-30T09:41:02.053Z",
        "barcode": "5784719087687",
        "qrCode": "[https://cdn.dummyjson.com/public/qr-code.png](https://cdn.dummyjson.com/public/qr-code.png)"
      },
      "images": [
        "[https://cdn.dummyjson.com/product-images/beauty/essence-mascara-lash-princess/1.webp](https://cdn.dummyjson.com/product-images/beauty/essence-mascara-lash-princess/1.webp)"
      ],
      "thumbnail": "[https://cdn.dummyjson.com/product-images/beauty/essence-mascara-lash-princess/thumbnail.webp](https://cdn.dummyjson.com/product-images/beauty/essence-mascara-lash-princess/thumbnail.webp)"
    },
    {
      "id": 2,
      "title": "Eyeshadow Palette with Mirror",
      "description": "The Eyeshadow Palette with Mirror offers a versatile range of eyeshadow shades for creating stunning eye looks. With a built-in mirror, it's convenient for on-the-go makeup application.",
      "category": "beauty",
      "price": 19.99,
      "discountPercentage": 18.19,
      "rating": 2.86,
      "stock": 34,
      "tags": [
        "beauty",
        "eyeshadow"
      ],
      "brand": "Glamour Beauty",
      "sku": "BEA-GLA-EYE-002",
      "weight": 9,
      "dimensions": {
        "width": 9.26,
        "height": 22.47,
        "depth": 27.67
      },
      "warrantyInformation": "1 year warranty",
      "shippingInformation": "Ships in 2 weeks",
      "availabilityStatus": "In Stock",
      "reviews": [
        {
          "rating": 5,
          "comment": "Great product!",
          "date": "2025-04-30T09:41:02.053Z",
          "reviewerName": "Savannah Gomez",
          "reviewerEmail": "savannah.gomez@x.dummyjson.com"
        },
        {
          "rating": 4,
          "comment": "Awesome product!",
          "date": "2025-04-30T09:41:02.053Z",
          "reviewerName": "Christian Perez",
          "reviewerEmail": "christian.perez@x.dummyjson.com"
        },
        {
          "rating": 1,
          "comment": "Poor quality!",
          "date": "2025-04-30T09:41:02.053Z",
          "reviewerName": "Nicholas Bailey",
          "reviewerEmail": "nicholas.bailey@x.dummyjson.com"
        }
      ],
      "returnPolicy": "7 days return policy",
      "minimumOrderQuantity": 20,
      "meta": {
        "createdAt": "2025-04-30T09:41:02.053Z",
        "updatedAt": "2025-04-30T09:41:02.053Z",
        "barcode": "9170275171413",
        "qrCode": "[https://cdn.dummyjson.com/public/qr-code.png](https://cdn.dummyjson.com/public/qr-code.png)"
      },
      "images": [
        "[https://cdn.dummyjson.com/product-images/beauty/eyeshadow-palette-with-mirror/1.webp](https://cdn.dummyjson.com/product-images/beauty/eyeshadow-palette-with-mirror/1.webp)"
      ],
      "thumbnail": "[https://cdn.dummyjson.com/product-images/beauty/eyeshadow-palette-with-mirror/thumbnail.webp](https://cdn.dummyjson.com/product-images/beauty/eyeshadow-palette-with-mirror/thumbnail.webp)"
    },
    ...
    ...
    ...
    ...
    ...
  "total": 194,
  "skip": 0,
  "limit": 30
}
```

**Success Criteria**
✅ Successfully fetch and display product data in a table
✅ Handle API errors gracefully
✅ Implement additional logic
✅ Improve table styling and UI/UX
✅ Follow good coding practices with clear file and code structure

Good luck! Remember, we're interested in your process as much as your final solution.

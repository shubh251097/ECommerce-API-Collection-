# E-Commerce API Testing

This project is a comprehensive **API testing implementation using Postman**, created to validate the core functionalities of an e-commerce application through REST APIs.

The Postman collection covers **user authentication, user profile management, product management, product search, product sorting, and shopping cart operations**. It includes multiple API requests with automated test scripts to validate HTTP status codes, response data, and business-related conditions.

The project also demonstrates practical API testing techniques such as **Bearer Token authentication, environment variables, dynamic test data, request chaining, response validation, and pre-request/test scripts**.

## 🔗 APIs Covered

| API                | Method | Endpoint                           |
| ------------------ | ------ | ---------------------------------- |
| Login API          | POST   | `/auth/login`                      |
| Get User Profile   | GET    | `/auth/me`                         |
| Get Products       | GET    | `/products`                        |
| Get Single Product | GET    | `/products/{product_id}`           |
| Search Product     | GET    | `/products/search?q=phone`         |
| Sort Products      | GET    | `/products?sortBy=title&order=asc` |
| Add New Product    | POST   | `/products/add`                    |
| Add to Cart        | POST   | `/carts/add`                       |
| Get Cart Details   | GET    | `/carts/31`                        |
| Get Cart Products  | GET    | `/carts/11`                        |

## 🧪 Testing Scope

The project demonstrates practical API testing concepts including:

* Functional API Testing
* Positive and Negative Testing
* Authentication and Bearer Token Validation
* HTTP Status Code Validation
* Response Body Validation
* JSON Request/Response Validation
* Product Search and Sorting Validation
* Cart Functionality Testing
* Environment Variables
* Dynamic Test Data
* API Request Chaining
* Automated Postman Test Scripts

## 🔄 API Chaining

The collection demonstrates end-to-end API chaining using Postman environment variables.

```text
Login API
   ↓
Access Token → token
   ↓
Get User Profile

Get Products
   ↓
Product ID → product_id
   ↓
Get Single Product / Add to Cart
   ↓
Cart ID → cart_id
   ↓
Get Cart Details / Get Cart Products
```

### Testing Approach

The collection uses **Postman JavaScript test scripts** to automate validations and verify expected API behavior. Dynamic values such as authentication tokens, product IDs, and cart IDs are captured from API responses and reused across subsequent requests.

This project demonstrates a structured approach to **functional API testing and end-to-end API workflow validation** using Postman.

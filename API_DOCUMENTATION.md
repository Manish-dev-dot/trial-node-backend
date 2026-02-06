# API Documentation

**Base URL**: `http://localhost:5000/api`

## Health Check
- **GET** `/health` - Check if API is running

---

## Users Endpoints

### Get All Users
- **GET** `/users`
- **Response**: `{ success: true, data: [...users] }`

### Get User by ID
- **GET** `/users/:id`
- **Response**: `{ success: true, data: {...user} }`

### Create User
- **POST** `/users`
- **Body**: `{ name: string, email: string, role: string }`
- **Response**: `{ success: true, data: {...newUser} }`

### Update User
- **PUT** `/users/:id`
- **Body**: `{ name?: string, email?: string, role?: string }`
- **Response**: `{ success: true, data: {...updatedUser} }`

### Delete User
- **DELETE** `/users/:id`
- **Response**: `{ success: true, data: {...deletedUser} }`

---

## Products Endpoints

### Get All Products
- **GET** `/products`
- **Response**: `{ success: true, data: [...products] }`

### Get Product by ID
- **GET** `/products/:id`
- **Response**: `{ success: true, data: {...product} }`

### Create Product
- **POST** `/products`
- **Body**: `{ name: string, price: number, category: string, stock: number }`
- **Response**: `{ success: true, data: {...newProduct} }`

### Update Product
- **PUT** `/products/:id`
- **Body**: `{ name?: string, price?: number, category?: string, stock?: number }`
- **Response**: `{ success: true, data: {...updatedProduct} }`

### Delete Product
- **DELETE** `/products/:id`
- **Response**: `{ success: true, data: {...deletedProduct} }`

---

## Test with Postman

1. Import this as a Collection or manually test the endpoints
2. Base URL: `http://localhost:5000/api`
3. All endpoints support JSON bodies where applicable

# CRUD Table Admin Panel with Sanctum API Laravel

Tugas Magang (Challenge Backend Laravel DOT Indonesia), Membuat Admin Panel Rest API 2 Table menggunakan token auth dengan Laravel Sanctum-API

## Screenshot

### Register

![github](https://user-images.githubusercontent.com/108115133/183000897-d44f019b-964b-4dc2-97c1-aee1823f940a.PNG)

### Login

![github](https://user-images.githubusercontent.com/108115133/183001042-2504b424-ff42-4c51-8269-8f61564e3aa1.PNG)

### List Customers

![github](https://user-images.githubusercontent.com/108115133/183001130-70230053-4a5d-49c5-9f09-effd79d836a3.PNG)

### List Orders

![github](https://user-images.githubusercontent.com/108115133/183001209-45f21a6b-77da-43d7-b63d-d098f978e575.PNG)

## Sanctum API with Token Auth

### Set Headers

![github](https://user-images.githubusercontent.com/108115133/183001517-4781454b-e99f-4732-a88d-e6b168e9c786.PNG)

### Register and get Token auth

```bash
  POST /api/register
```

![github](https://user-images.githubusercontent.com/108115133/183002492-7533424a-2d80-40aa-b94d-36db8910ab4b.PNG)

### Set auth Token in Bearer Token

![github](https://user-images.githubusercontent.com/108115133/183002663-7cffccb7-f4ab-4738-8501-ef8ead0b9e90.PNG)

### Logout

```bash
  POST /api/logout
```

![github](https://user-images.githubusercontent.com/108115133/183007753-2bf016bb-269b-460e-8cba-6c87c0c5ddd4.PNG)

### Login

```bash
  POST /api/login
```

![github](https://user-images.githubusercontent.com/108115133/183007819-b997c740-890b-44b1-b071-4201b7452143.PNG)

### With Auth Token can access all Routes

```bash
  # Public Routes
    POST /api/register
    POST /api/login
    
  - Customers
    GET /api/customers
    GET /api/customers/{id}
    GET /api/customers/search/{name}
    
  - Posts
    GET /api/posts
    GET /api/posts/{id}
    GET /api/posts/search/{title}
    
  # Protected Routes
    POST /api/logout
    
  - Customers
    POST /api/customers
    PUT /api/customers/{id}
    DELETE /api/customers/{id}
    
  - Posts
    POST /api/posts
    PUT /api/posts/{id}
    DELETE /api/posts/{id}
```

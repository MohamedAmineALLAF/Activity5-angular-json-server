# Angular project with json server
<hr>

<br>

First of all to user json-server we need to install it as the following :<br>

```markdown
npm i json-server
```

and for json-server-auth we need : <br>

```markdown
npm i json-server-auth
```

and then we need to create a folder ****'data'**** and inside it, we're going to create ****'db.json'**** file as the following :<br>

```json
{
"products": [
{
"name": "Nawfal",
"price": 0,
"checked": true,
"id": 4
},
{
"name": "Marouane",
"price": 1,
"checked": false,
"id": 8
},
{
"name": "Abrak",
"price": 799,
"checked": false,
"id": 12
},
{
"name": "Tahri",
"price": 999,
"checked": true,
"id": 16
},
{
"name": "MSI GF63",
"price": "960",
"checked": true,
"id": 20
},
{
"name": "PS5",
"price": "699",
"checked": true,
"id": 24
},
{
"name": "IPhone 14 pro max",
"price": "1500",
"checked": false,
"id": 28
},
{
"name": "Oussama",
"price": "899",
"checked": true,
"id": 32
},
{
"name": "newP",
"price": "1",
"checked": true,
"id": 33
},
{
"name": "newProduct",
"price": "232322323",
"checked": true,
"id": 34
}
],
"users": [
{
"id": "user1",
"password": "MTIzNA==",
"token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiJ1c2VyMSIsIm5hbWUiOiJPdXNzYW1hIiwiZW1haWwiOiJ1c2VyMUBnbWFpbC5jb20iLCJpYXQiOjE3MDAyODkwMjIsInJvbGVzIjpbIlVTRVIiXX0.876Nkwsh3nT38e4r8dV8SEMjGcjqg4H5ClFWiXBibXs"
},
{
"id": "admin",
"password": "MTIzNA==",
"token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiJhZG1pbiIsIm5hbWUiOiJPdXNzYW1hIiwiZW1haWwiOiJhZG1pbkBnbWFpbC5jb20iLCJpYXQiOjE3MDAyODkwMjIsInJvbGVzIjpbIlVTRVIiLCJBRE1JTiJdfQ.4c0Gyx4sRiwN9D8rtw-4HCnL7TaZl4INKto0W9n0Wz8"
}
]
}
```
and the last thing is the cmd to lunch json server api : <br>

```markdown
json-server -w data/db.json -p 9000
```

<br>

<br>

The JWT I created for admin with roles **'ADMIN'** and **'USER'**

![Admin JWT](captures/jwt-admin.png)

<br>

The login page:

![Login Page](captures/auth-admin.png)

<br>

As an **'ADMIN'**, he can check all products, modify, and delete each of them:

![Admin Products](captures/products.png)

<br>

To create a product, there are some requirements we should respect:

![Create Product](captures/create.png)

<br>

A message with pipe JSON shows when the product is created:

![Product Created](captures/product-created.png)

<br>

The JWT I created for user1 with role **'USER'**

![User JWT](captures/jwt-user.png)

<br>

As a **'USER'**, he can only see the products:

![User Products](captures/products-user.png)

<br>

Once the **'USER'** is trying to create a product, he gets this **"notAuthorized"** page:

![Not Authorized](captures/not-authorized.png)


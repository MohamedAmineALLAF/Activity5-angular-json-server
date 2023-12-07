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

The JWT I created for admin with roles ****'ADMIN'**** and ****'USER'****

<img src="captures/jwt-admin.png">

<br>

The login page :

<img src="captures/auth-admin.png">

<br>

as an ****'ADMIN'**** he can check all products, modify and delete each of'em

<img src="captures/products.png">

<br>

to create a product there is some requires we should respect 

<img src="captures/create.png">

<br>

A message with pipe json shows when the product is created

<img src="captures/product-created.png">

<br>

The JWT I created for user1 with role ****'USER'****


<img src="captures/jwt-user.png">

<br>

as an ****'USER'**** he can only see the products


<img src="captures/products-user.png">

<br>

Once the ****'USER'**** is trying to create a product he gets this ***"notAuthorized"*** page

<img src="captures/not-authorized.png">

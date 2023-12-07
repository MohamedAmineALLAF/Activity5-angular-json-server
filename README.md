# Angular project with json server
<hr>

<br>

to install json-server run the command :<br>

```markdown
npm i json-server
```

and for json-server-auth we need : <br>

```markdown
npm i json-server-auth
```


and launch json server api by running : <br>

```markdown
json-server -w data/db.json -p 9000
```

<br>

<br>

The JWT I created for admin with roles **'ADMIN'** and **'USER'**

![Admin JWT](captures/admin-json.jpg)

<br>

The login page:

![Login Page](captures/login-page.jpg)

<br>

As an **'ADMIN'**, he can check all products, modify, and delete each of them:

![Admin Products](captures/admin-products.jpg)

<br>

To create a product, we get this message:

![Create Product](captures/save-product.jpg)

<br>


JWT created for user1 with role **'USER'**

![User JWT](captures/user-jwt.jpg)

<br>

As a **'USER'**, he can only see the products:

![User Products](captures/user-show.jpg)

<br>

Once the **'USER'** is trying to create a product, he gets this **"notAuthorized"** page:

![Not Authorized](captures/not-authorized.jpg)


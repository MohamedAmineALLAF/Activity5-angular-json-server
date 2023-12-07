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

![Admin JWT](captures/jwt-admin.jpg)

<br>

The login page:

![Login Page](captures/auth-admin.jpg)

<br>

As an **'ADMIN'**, he can check all products, modify, and delete each of them:

![Admin Products](captures/products.jpg)

<br>

To create a product, there are some requirements we should respect:

![Create Product](captures/create.jpg)

<br>

A message with pipe JSON shows when the product is created:

![Product Created](captures/product-created.jpg)

<br>

The JWT I created for user1 with role **'USER'**

![User JWT](captures/jwt-user.jpg)

<br>

As a **'USER'**, he can only see the products:

![User Products](captures/products-user.jpg)

<br>

Once the **'USER'** is trying to create a product, he gets this **"notAuthorized"** page:

![Not Authorized](captures/not-authorized.jpg)


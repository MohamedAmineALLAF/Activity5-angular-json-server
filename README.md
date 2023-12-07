# Angular project with json server

This Angular project is a comprehensive web application that seamlessly integrates with a JSON Server, providing a robust backend for data management. The project leverages the power of Angular, a widely used front-end framework, to create a dynamic and interactive user interface.

## Technologies Used

- **Angular:** The core of the front-end development, Angular facilitates the creation of a modular and scalable structure for the application. It enables the seamless integration of components, services, and routing.

- **JSON Server:** Serving as the backend, JSON Server is utilized to simulate a RESTful API and manage data through a JSON-based database. This simplifies the development process by providing a lightweight and easy-to-use server.

- **JSON Server Auth:** An extension for JSON Server that adds authentication capabilities, ensuring secure access to different parts of the application.


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


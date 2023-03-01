
# Aarogya Setu Backend

This is the backend of the Aarogya Setu application, which allows users to log in, book their slots for COVID-19 vaccination, and cancel their slots. The backend is built with Node.js and Express.js, utilizing Mongoose for database management and MongoDB as the database. The application uses JWT tokens for authentication and authorization.



## Features
 
### User Authentication
Users can register and log in to the application using their email and password. User passwords are hashed and stored securely in the database using the bcrypt library.

### User Bookings
Users can book their slots for COVID-19 vaccination, specifying the date and time they wish to receive the vaccination. Users can also cancel their bookings if necessary, freeing up the slot for other users to book. The application uses JWT tokens to authenticate users and ensure that users can only book or cancel their own slots.

### Admin Management
Admins can create slots for vaccination and view the status of other users who have booked their slots. Admins are authenticated using JWT tokens and can only perform admin actions if their token includes the appropriate admin permissions.
 
### JWT Token-based Authentication
The application uses JWT tokens for authentication and authorization, ensuring the security of user data. JWT tokens are generated for each user upon registration and login, and are used to authenticate users and ensure that only authenticated users can book or cancel their slots. JWT tokens are also used to authenticate admins and ensure that only admins can perform admin actions.

## Technologies Used

### Node.js
Node.js is a popular server-side JavaScript runtime environment. It provides an event-driven, non-blocking I/O model that makes it lightweight and efficient.

### Express.js
Express.js is a popular Node.js web application framework used for building APIs and web applications. It provides a set of robust features for building scalable and maintainable web applications.

### Mongoose
Mongoose is a popular Object Data Modeling (ODM) library used for managing MongoDB databases. It provides a straightforward way to define data models and interact with MongoDB databases.

### MongoDB
MongoDB is a popular NoSQL database used for storing and managing data. It provides a flexible schema that allows for easy scaling and horizontal growth.

### JWT
JSON Web Tokens (JWT) are used for authentication and authorization. JWT is a stateless, standardized way of securely transmitting information between parties as a JSON object.
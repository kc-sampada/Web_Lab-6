LAB 6 — Todo API with User Authentication (FastAPI with ORM and Migrations)

1. Created a Todo model linked to the User model using a foreign key on user id.
2. Applied Alembic migrations to add the todos table to the database.
3. Built routes to create, read, update and delete todos for the authenticated user.
4. Used the JWT token from the login response to identify the current user on each request.
5. Filtered todo queries by user id so each user only sees their own todos.
6. Organized code into separate route and controller files following the structure from Lab 5.

This lab was done to extend the authentication system from Lab 5 into a fully functional protected API. Displaying all todos from the database regardless of user would be a privacy issue, so filtering by user id was necessary to ensure each user only accesses their own data. Using the authenticated user's id from the JWT token to scope database queries is the standard pattern in real world APIs. The foreign key relationship between todos and users enforced data integrity at the database level. Reusing the project structure from Lab 5 kept the codebase consistent and easy to navigate. This lab completed the full stack foundation by connecting a secure backend API to user-specific data.

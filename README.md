### Food ordering application

The food ordering application is implemented using ReactJS (Hooks) library and Java Spring Boot framework (Hibernate, Spring Secuirty with JSON Web token, REST API) with some additional libraries (Bootstrap, AXIOS, Sweetalert, Redux and few more).

### Project specification

The main purpose of the application is to enable users to view restaurant menu, place food orders, then track the status of their orders, which can be updated by employees. The system consists of three user roles with specific capabilities:
- ADMIN
- EMPLOYEE
- USER

The application can also be accessed by unregistered users, who have the following abilities:
- Register an account
- Browse the menu, select a type of the meal, and view the complete offerings within that type
- Specify quantities and then add items to the cart
- Confirm the final order by inserting their address and phone number
- After successfully placing the final order, users will receive a message containing a link to track the status of their order

Registered users with the *USER* role can log into the system using their username and password. They have the following abilities:
- Update their personal information
- Order food similar to unregistered users, but without the need to enter their address and phone number since their data is already saved in the database.
- Receive a 10% discount on every order
- View their active orders (with *ORDERED* and *IN PREPARATION* status)
- View the history of their orders (with *IN DELIVERY* status)

Users with the *EMPLOYEE* role have the following abilities:
- Review all incoming orders and change their status to *IN PREPARATION* or *IN DELIVERY*, depending on whether the orders are being prepared or in the process of delivery.
- View the history of all orders.

Users with the *ADMIN* role have the following abilities:
- Create, delete (logically) and update meal types in the database (including uploading images)
- Create, delete (logically) and update meals (including uploading images)
- Logically delete users (change their isDeleted status, their data remains in the database)
- View active final orders
- Delete final orders and all their ordered items from the database
- View the order history
- Create, delete, and update employee data (users with the *EMPLOYEE* role)

Application has fully responsive design for users who order the food.

### Application UI preview:

![1](https://github.com/shivam-0105/food-ordering-app/assets/70219870/aee579fc-3774-40ed-af02-f4da760bce27)
![2](https://github.com/shivam-0105/food-ordering-app/assets/70219870/43835850-2468-4e6e-8ae9-2396da6ffc8a)
![3](https://github.com/shivam-0105/food-ordering-app/assets/70219870/a9e07cbd-062e-4317-a015-ef744ecb6e7c)

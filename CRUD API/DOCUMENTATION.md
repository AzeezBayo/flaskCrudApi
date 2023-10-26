# REST API Development THAT PERFORM CRUD OPERATION
## Engine
SQLite was use as the database management system, scalable DBMS like postgreSQL can be use.
## CREATE
Copy this above url to postman or any endpoint, you can supply raw json text or form-data.
*Note*: Send POST request and it takes only string other data type will return error
```
Usage: /api
{
    "name": "Person Name"
}
on success: {'message': 'User created successfully'}
on failure: {'error': 'Name is required'}
```
## READ
Send GET Request to retrieve all users or a specific user
```
Usage: /api/user_id or /api
on success: [{'user_id': user_id, 'name': name}]
on failure: {'error': 'User not found'}
```
## UPDATE
Make use of the PUT Request to modify data in the table
```
Usage: /api/user_id
on success: {'message': 'User updated successfully'}
on failure: {'error': 'Name is required'}
```
## DELETE
Send DELETE Request to Remove entity from database.
```
Usage: /api/user_id
on success: {'message': 'User deleted successfully'}
on error: {'error': 'User not found'}
```

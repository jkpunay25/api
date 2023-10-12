"# api" 
# API Name
A: Demo API

Brief description of your API.
A: The "Demo API" is a simple RESTful API for managing names in a MySQL database. It supports creating, retrieving, updating, and deleting name records.
 
## API
Description
A: This API is a basic RESTful API for managing names in a database. It provides endpoints for creating, retrieving, updating, and deleting name records.

Provide a more
detailed explanation of what your API does, its purpose, and any key features.
A: The "Demo API" is a basic RESTful API for managing name records in a MySQL database, supporting standard CRUD operations: Create, Read, Update, and Delete. While it provides a simple framework, it lacks advanced features like data validation and secure database connections, making it suitable primarily for educational purposes and as a starting point for more complex API development.
 


## API
Endpoints
Describe the
available endpoints, their functions, and the required parameters.

1. Insert Data (POST/postName)
   - Description: Insert a new name into the database.
   - Method: POST
   - Required Parameters:
       - fname'(string): First name.
       - lname'(string): Last name.
2. Retrieve Data (GET/getName)
   - Description: Retrieve a list of names from the database.
   - Method: GET
3. Update Data (POST/updateName)
   - Description: Update an existing name record in the database.
   - Method: POST
   - Required Parameters:
       - 'id' (int): The unique identifier of the name.
       - 'fname' (string): New first name.
       - 'lname' (string): New last name.
4. Delete Data(POST/deleteName)
   - Description: Delete a name record from the database.
   - Method: POST
   - Required Parameters:
       - 'id' (int): The unique identifier of the name to be deleted.

## Request
Payload
Explain the
structure of the request payload, including any required or optional fields.
You can use JSON examples to illustrate.
A:
1. Insert Data (POST/postName)
- Structure of the request payload:
{
  "fname": "Kathlene",
  "lname": "Punay"
}

2. Update Data (POST/updateName)
- Structure of the request payload:
{
    "id": 1,
    "fname": "Vanesa",
    "lname": "Salvador"
}


 
## Response
Describe the
structure of the API response, including possible status codes and JSON
examples.
A:
- Structure of the API response:
Success (Status Code: 200):
{
    "status": "success",
    "data": {...}  // Data varies based on the endpoint
}

Error (Status Code: 500):
{
    "status": "error",
    "message": "An error message here"
}

 
 
## Usage
Provide code
examples or instructions on how to use your API.
A: You can use this API to perform CRUD operations on name records in the database. Below are some code examples:
Insert Data:
curl -X POST http://your-api-url/postName -d '{"fname": "Kathlene", "lname": "Punay"}'

Retrieve Data:
curl http://your-api-url/getName

Update Data:
curl -X POST http://your-api-url/updateName -d '{"id": 1, "fname": "Vanesa", "lname": "Salvador"}'

Delete Data:
curl -X POST http://your-api-url/deleteName -d '{"id": 1}'

## License
Mention the
license under which your API is distributed.

A: This API is distributed under the MIT License.
 
## Contributors
List
contributors or give credit to any external libraries or resources used.

A: Dr. Manny R. Hortizuela

## Contact
Information

Name: Kathlene Punay

"# api" 
# API Name
- Demo API

Brief description of your API.
- The "Demo API" is a simple RESTful API for managing names in a MySQL database. It supports creating, retrieving, updating, and deleting name records.
 
## API
Description
- This API is a basic RESTful API for managing names in a database. It provides endpoints for creating, retrieving, updating, and deleting name records.

Provide a more
detailed explanation of what your API does, its purpose, and any key features.
- The "Demo API" is a basic RESTful API for managing name records in a MySQL database, supporting standard CRUD operations: Create, Read, Update, and Delete. While it provides a simple framework, it lacks advanced features like data validation and secure database connections, making it suitable primarily for educational purposes and as a starting point for more complex API development.
 


## API
Endpoints
Describe the
available endpoints, their functions, and the required parameters.

1. Insert Data (POST/postName) http://127.0.0.1/api/public/postName
   - Description: Insert a new name into the database.
   - Method: POST
   - Required Parameters:
       - fname'(string): First name.
       - lname'(string): Last name.
2. Retrieve Data (GET/getName) http://127.0.0.1/api/public/printName
   - Description: Retrieve a list of names from the database.
   - Method: GET
3. Update Data (POST/updateName) http://127.0.0.1/api/public/updateName
   - Description: Update an existing name record in the database.
   - Method: POST
   - Required Parameters:
       - 'id' (int): The unique identifier of the name.
       - 'fname' (string): New first name.
       - 'lname' (string): New last name.
4. Delete Data(POST/deleteName) http://127.0.0.1/api/public/deleteName
   - Description: Delete a name record from the database.
   - Method: POST
   - Required Parameters:
       - 'id' (int): The unique identifier of the name to be deleted.

## Request
Payload
Explain the
structure of the request payload, including any required or optional fields.
You can use JSON examples to illustrate.

JSON Payload Name:

JSON Payload postName:
Request payload:
{ "lname":"hortizuela", "fname":"manny" }
JSON Payload printName:

Request payload:

JSON Payload updateName:

Request payload:
{ "id":1, "lname":"wick", "fname":"john" }
JSON Payload deleteName:

Request payload:
{ "id":1 }


 
## Response
Describe the
structure of the API response, including possible status codes and JSON
examples.
JSON Payload Name:

Response payload:
{ "status":"success","data":null }
JSON Payload printName:

Response payload:
{ "status":"success","data":["lname":"hortizuela","fname":"manny","lname":"licayan","fname":"arnold"] }
JSON Payload updateName:

Response payload:
{ "status":"success","data":null }
JSON Payload deleteName:

Response payload:
{ "status":"success","data":null }
 
 
## Usage
Provide code
examples or instructions on how to use your API.

Using Postman to Interact with the API

Launch Postman: Ensure that Postman is installed and ready for use on your system.

Insert Data into the Database:

Choose the HTTP method as "POST."
Input the URL: http://127.0.0.1/api/public/postName.
In the request body, provide the parameters "fname" and "lname" with the values you want to insert.
Click the "Send" button to execute the request.
Update Existing Data:

Select the HTTP method as "POST."
Enter the URL: http://127.0.0.1/api/public/updateName.
Include the parameters "id," "fname," and "lname" in the request body with the updated values.
Click "Send" to submit the request.
Retrieve Data from the Database:

Choose the HTTP method as "GET."
Specify the URL: http://127.0.0.1/api/public/printName.
Keep the request body empty, as no additional parameters are needed.
Click "Send" to retrieve the data.
Delete Data from the Database:

Set the HTTP method to "POST."
Enter the URL: http://127.0.0.1/api/public/deleteName.
In the request body, include the "id" parameter with the ID of the data you wish to delete.
Click "Send" to initiate the deletion request.

## License
Mention the
license under which your API is distributed.

- No License.
 
## Contributors
List
contributors or give credit to any external libraries or resources used.

Dr. Manny Hortizuela:
 - some codes
 - structure of the database
 - payloads
 - others

## Contact
Information

Name: Kathlene Punay
Email: kathlene.punay@student.dmmmsu.edu.ph
Number: 09474892584

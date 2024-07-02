## Postman collections from test tasks

### Petstore API
Task: create a collection in Postman. Queries that should be in the collection:
1. Create a new pet (POST /pet method), and fill in all the keys with your example values. Write a script on the tests tab that takes the ID of the created pet from the response body and writes it to the collection.
2. Write a script that takes the name and tags of the pet from the response body and writes it to the collection. Specify a check on the Tests tab, that the tag name from the request body equals the tag name from the server response body.
3. Get pet information by id (GET /pet/{petId} method), using the previously recorded id pet variable from the collection in the request.
On the tests tab, write a script that will send the following request “Updates a pet in the store with form data” (method POST /pet/{petId}) to update the “status” key to “sold” (sold).
Hint: use pm.sendRequest
4. As for negative checks, create additional queries:
Pet ID is invalid when created - error 400 (bad input)
Pet ID does not exist upon receipt - error 404 (Pet not found)
Unsupported data format when creating - 415 error Unsupported Media Type
When creating a pet, what must be done to display this 500 Server Error?


# API-Testing

Below some test cases I made for API Testing 

_____________________________________________________________________________________________________________________________________________

Title : Create an API 

Description : Add a new pet to the store 

Preconditions: Open the Postman website: https://speeding-meadow-227188.postman.co & log in with your username and password  

Steps to reproduce : 

1. Click on "Workspaces", then "My Workspace"
2. Click the "New" button
3. Select "HTTP" request
4. Select "POST" from droplist
5. Insert "https://petstore.swagger.io/v2/pet"
6. Click on "Body"
7. Select "JSON" from the blue droplist
8. Go to "https://petstore.swagger.io/#/pet/addPet"
9. Click on the second "POST" button from the pet section
10. Copy required body object from the black textbox
11. Paste on Postman the copied text in cell
12. Complete the textbox with details: id, name, status for the new pet
13. Click the "Send" button

Expected results: The new pet has been successfully added with Status: 200 OK and all the details are displayed in the Body textbox.

Test data: id: 1 & name: "Rex" 

Environment : Google Chrome


![post method](https://github.com/dicacristian/API-Testing/assets/85904271/50631e2d-8baa-4e22-8eb3-804baf26db45)
_____________________________________________________________________________________________________________________________________________

Title : Update an API 

Description: Update an existing pet 

Preconditions: Open the Postman website: https://speeding-meadow-227188.postman.co & log in with your username and password  

Steps to reproduce : 

1. Click on "Workspaces", then "My Workspace"
2. Click the "New" button
3. Select "HTTP" request
4. Select "PUT" from droplist
5. Add https://petstore.swagger.io/v2/pet into requested URL textbox
6. Go to https://petstore.swagger.io/#/pet/updatePet and copy the required body
7. Paste on Postman the copied text in Body/raw/json
8. Update the "name" with "Tommy" and ID with "20"
9. Click the "Send" button

Expected results: The name and ID field has changed successfully with those modified

Environment : Google Chrome


_____________________________________________________________________________________________________________________________________________







   


# API-Testing

Below some test cases I made for API Testing 

_____________________________________________________________________________________________________________________________________________

Title: Find an API

Description: Find a pet by ID after the pet has been created

Preconditions: Open the Postman website: https://speeding-meadow-227188.postman.co & log in with your username and password

Steps to reproduce: 

1. Click on "Workspaces", then "My Workspace"
2. Click the "New" button
3. Select "HTTP" request
4. Select "Get" from droplist
5. Copy base URL from Swagger website "https://petstore.swagger.io/"
6. Add "v2/pet/2"
7. Hit the "Send" button

   Expected results: All the details about the pet are displayed

   Environment : Google Chrome

   ![get method](https://github.com/dicacristian/API-Testing/assets/85904271/a56036da-6bf7-4201-bb11-b7c94af276f9)



_____________________________________________________________________________________________________________________________________________

Title : Including an API that does not exist 

Description : Test the "Get" method with letters instead of number. 
Steps to reproduce: 

1. Click on "Workspaces", then "My Workspace"
2. Click the "New" button
3. Select "HTTP" request
4. Select "Get" from droplist
5. Copy base URL from Swagger website "https://petstore.swagger.io/"
6. Add "v2/pet/dsafas"
7. Hit the "Send" button

Expected results: The message "For input string: \"dsafas/" with status 404 is displayed in the Body textbox

![test failed](https://github.com/dicacristian/API-Testing/assets/85904271/904abc62-fba6-45a8-b5b0-63281212da6a)


_____________________________________________________________________________________________________________________________________________

Title : Create an API 

Description : Add a new pet to the store 

Preconditions: Open the Postman website: https://speeding-meadow-227188.postman.co & log in with your username and password  

Steps to reproduce : 

1. Click on "Workspaces", then ""My Workspace"
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

![post method](https://github.com/dicacristian/API-Testing/assets/85904271/50631e2d-8baa-4e22-8eb3-804baf26db45)


_____________________________________________________________________________________________________________________________________________







   


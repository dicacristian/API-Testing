# API-Testing

Below some test cases I made for API Testing 

_____________________________________________________________________________________________________________________________________________

**Title** : Create an API 

**Description** : Add a new pet to the store 

**Preconditions** : Open the Postman website: https://speeding-meadow-227188.postman.co & log in with your username and password  

**Steps to reproduce** : 

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

**Expected results** : The new pet has been successfully added with Status: 200 OK and all the details are displayed in the Body textbox.

**Test data** : id: 1 & name: "Rex" 


![post method](https://github.com/dicacristian/API-Testing/assets/85904271/50631e2d-8baa-4e22-8eb3-804baf26db45)
_____________________________________________________________________________________________________________________________________________

**Title** : Update an API 

**Description** : Update an existing pet 

**Preconditions** : Open the Postman website: https://speeding-meadow-227188.postman.co & log in with your username and password  

**Steps to reproduce** : 

1. Click on "Workspaces", then "My Workspace"
2. Click the "New" button
3. Select "HTTP" request
4. Select "PUT" from droplist
5. Add https://petstore.swagger.io/v2/pet into requested URL textbox
6. Go to https://petstore.swagger.io/#/pet/updatePet and copy the required body
7. Paste on Postman the copied text in Body/raw/json
8. Update the "name" with "Tommy" and ID with "20"
9. Click the "Send" button

**Expected results** : The name and ID field has changed successfully with those modified


![image](https://github.com/dicacristian/API-Testing/assets/85904271/a19ec52c-b904-42c0-b7fb-f9a2a1e4302f)


_____________________________________________________________________________________________________________________________________________

**Title** : Delete an existing API 

**Preconditions** : Open the Postman website: https://speeding-meadow-227188.postman.co & log in with your username and password  

**Steps to reproduce**  : 

1. Click on "Workspaces", then "My Workspace"
2. Click the "New" button
3. Select "HTTP" request
4. Select "Delete" from droplist
5. Copy "https://reqres.in/api/users/2" into  requested URL textbox
6. Click the "Send" button

**Expected results** : The elements deleted successfully 



![delete api](https://github.com/dicacristian/API-Testing/assets/85904271/5c879f30-9b02-47ac-85c1-cc1a792f7741)

Source : https://reqres.in/

![deleted api reqres](https://github.com/dicacristian/API-Testing/assets/85904271/3934544e-786c-4216-a78b-bffea07ba450)


_____________________________________________________________________________________________________________________________________________
   
**Title** : Find an API

**Description** : Find a pet by ID after the pet has been created


**Preconditions** : Open the Postman website: https://speeding-meadow-227188.postman.co & log in with your username and password  

**Steps to reproduce**  :

 1. Open a new API: Workspaces/My Workspaces/ New/ Select "HTTP" request
 2. Select "GET" from droplist
 3. Insert the POST URL created before for a new pet / https://petstore.swagger.io/v2/pet
 4. Copy "https://petstore.swagger.io/v2/pet/1" into requested URL textbox
 5. Click on "Send" button

**Expected results** : All the details about the pet are displayed 

![image](https://github.com/dicacristian/API-Testing/assets/85904271/0537dc13-4736-45f5-9f33-f2628689e417)


_____________________________________________________________________________________________________________________________________________

**Title** : Find a API with 3 parameters 

**Description** : Finding an API with 3 parameters which in our case are the name of the movie: Batman, the type which is serial and as format we chose json

****Preconditions** : Open the Postman website: https://speeding-meadow-227188.postman.co & log in with your username and password  

**Steps to reproduce**  :

 1. Open a new API: Workspaces/My Workspaces/ New/ Select "HTTP" request
 2. Select "GET" from droplist
 3. Insert the GET URL created before for a new pet / https://www.omdbapi.com/?apikey=[56fe3e3d]&s=Batman&type=series&r=json
 4. Press on "Authorization", then click on "Need help authorizing with OMDb API?"
 5. Copy "56fe3e3d" on the section "Enter the API Key here"
 6. Press the "Send" button

**Expected results** : All the details about the Batman series are displayed 


![image](https://github.com/dicacristian/API-Testing/assets/85904271/305c8551-e41c-446d-afc0-e32744046685)

_____________________________________________________________________________________________________________________________________________

**Title** : Read all API data base 

**Description** : Read all API data base for searching more easier an specific ID 

****Preconditions** : Open the Postman website: https://speeding-meadow-227188.postman.co & log in with your username and password  

**Steps to reproduce**  :

   1. Open a new API: Workspaces/My Workspaces/ New/ Select "HTTP" request
   2. Select "GET" from droplist
   3. Insert the GET URL for reading users : http://qachallenge.ro/api/test_api.php?action=fetch_all
   4. Press the "Send" button

**Expected result** :  All users are displayed 

![image](https://github.com/dicacristian/API-Testing/assets/85904271/4f397bbe-d078-4a85-be79-1bfff25b4c47)


_____________________________________________________________________________________________________________________________________________

**Title** : Read a specific user

**Description** : Searching a specific user by ID 

****Preconditions** : Open the Postman website: https://speeding-meadow-227188.postman.co & log in with your username and password  

**Steps to reproduce** :  

  1. Open a new API: Workspaces/My Workspaces/ New/ Select "HTTP" request
  2. Select "GET" from droplist
  3. Insert the GET URL for reading a specific user : http://qachallenge.ro/api/test_api.php?action=fetch_single&id=628
  4. Press the "Send" button

 **Expected result** : The specific user is displayed


![image](https://github.com/dicacristian/API-Testing/assets/85904271/7f9540e1-7321-4a0a-b9d1-2a874c4680e5)


_____________________________________________________________________________________________________________________________________________

**Title** : Create a user 

**Description** : Create a user based on our API

****Preconditions** : Open the Postman website: https://speeding-meadow-227188.postman.co & log in with your username and password  

**Steps to reproduce** :  

   1. Open a new API: Workspaces/My Workspaces/ New/ Select "HTTP" request
   2. Select "POST" from droplist
   3.  Insert the POST URL for creating a user : http://qachallenge.ro/api/test_api.php?action=insert
   4.  Press the "Send" button

**Expected result** : The user was created


![image](https://github.com/dicacristian/API-Testing/assets/85904271/f8e583a9-daba-424c-b4e5-f3c43c755178)


_____________________________________________________________________________________________________________________________________________

**Title** : Update a user 

**Description** : Update a user based on our API

****Preconditions** : Open the Postman website: https://speeding-meadow-227188.postman.co & log in with your username and password  

**Steps to reproduce** :  

   1. Open a new API: Workspaces/My Workspaces/ New/ Select "HTTP" request
   2. Select "POST" from droplist
   3.  Insert the POST URL for creating a user : http://qachallenge.ro/api/test_api.php?action=insert
   4.  Press the "Send" button

**Expected result** : The phone number was added successfully

![image](https://github.com/dicacristian/API-Testing/assets/85904271/75ed7d27-55bc-4b1f-8533-03f0b0b032a5)


_____________________________________________________________________________________________________________________________________________

**Title** : Deleting a user parameter

**Description** : I chose to delete email as our user parameter

**Preconditions** : Open the Postman website: https://speeding-meadow-227188.postman.co & log in with your username and password  

**Steps to reproduce** :

   1. Open a new API: Workspaces/My Workspaces/ New/ Select "HTTP" request
   2. Select "Delete" from droplist
   3.  Insert the DELETE URL for creating a user : http://qachallenge.ro/api/test_api.php?action=insert
   4.  Press the "Send" button

**Expected result** : The specific parameter, in our case the email was successfully deleted

![image](https://github.com/dicacristian/API-Testing/assets/85904271/49aea2c2-6804-4f8c-a014-a6532f1b6667)

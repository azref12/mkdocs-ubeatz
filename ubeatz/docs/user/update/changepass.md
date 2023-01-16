## Change Password 

### Endpoint
````
[PUT] url/user/changepassword/ 
````

### PUT Method 
For *PUT* method, use this ``json`` file with the format below to change password.
````
{
    "id": "(confidential data)",
    "password": "(confidential data)"
}
````
### Result 
````
{
    "message": "successfully",
    "status": true,
    "count": 1,
    "results": "Change Password Success"
}
````
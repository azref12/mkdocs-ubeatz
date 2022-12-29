## Change Password 
Endpoint
````
    url/user/changepassword/ [PUT]
````
use this ``json`` file with the format below to change password
````
{
    "id": "2",
    "password": "12345678"
}
````
## Result 
````
{
    "message": "successfully",
    "status": true,
    "count": 1,
    "results": "Change Password Success"
}
````
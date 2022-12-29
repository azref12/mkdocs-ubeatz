## Change Phone Number
Endpoint
````
    url/user/changephonenumber/ [PUT]
```` 
use this ``json`` file with the format below to change phone number
````
{
    "username": "anonim12",
    "phone_number": "+6281234567892"
}
````
## Result
````
{
    "message": "successfully",
    "status": true,
    "count": 1,
    "results": "User has been change phone number"
}
````
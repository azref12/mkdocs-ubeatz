## Change Phone Number

### Endpoint
````
[PUT] url/user/changephonenumber/ 
````

### PUT Method 
For *PUT* method, use this ``json`` file with the format below to change phone number.
````
{
    "username": "(confidential data)",
    "phone_number": "(confidential data)"
}
````
### Result
````
{
    "message": "successfully",
    "status": true,
    "count": 1,
    "results": "User has been change phone number"
}
````
## Sign Up

### Endpoint
````
[POST] url/user/user 
````

### POST Method
Use this ``json`` file with the format below to sign up.
````
{
    "first_name": "-",
    "last_name": "-",
    "username": "(confidential data)",
    "email": "(confidential data)",
    "phone_number": "(confidential data)",
    "password": "(confidential data)",
    "password2": "(confidential data)",
    "pin": "",
    "referral_code" : "(confidential data)"
}
````
### Result
```` 
{
    "message": "successfully",
    "status": true,
    "count": 1,
    "results": {
        "master": [
            {
                "id": (confidential data),
                "reward": 0,
                "point": 0,
                "coin": 0,
                "phone_number": "(confidential data)",
                "pin": "(confidential data)",
                "code": (confidential data),
                "status": 0,
                "count_referal": 0,
                "idgetplus": "0",
                "membergetplus": "0",
                "extradata": null
            }
        ]
    }
}
````
### Error condition
````
If email format doesn't match.
{
    "message": "unsuccessfully",
    "status": false,
    "count": 1,
    "results": "Username is already registered"
}

If password doesn't match.
{
    "message": "unsuccessfully",
    "status": false,
    "count": 1,
    "results": "Password Minimum 8 Character"
}

If username has been registered.
{
    "message": "unsuccessfully",
    "status": false,
    "count": 1,
    "results": "Username is already registered"
}

If email has been registered.
{
    "message": "unsuccessfully",
    "status": false,
    "count": 1,
    "results": "Email is already registered"
}
````
## Sign Up

Endpoint
````
    url/user/user [POST]
````
use this ``json`` file with the format below to sign up
````
{
    "first_name": "-",
    "last_name": "-",
    "username": "anonim12",
    "email": "anonim12@gmail.com",
    "phone_number": "+6281234567891",
    "password": "123123123",
    "password2": "123123123",
    "pin": "",
    "referral_code" : "zref"
}
````
## Result
```` 
{
    "message": "successfully",
    "status": true,
    "count": 1,
    "results": {
        "master": [
            {
                "id": 2,
                "reward": 0,
                "point": 0,
                "coin": 0,
                "phone_number": "+6281234567891",
                "pin": "JLN8WO",
                "code": 3920,
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
## Error condition
````
#response if email format does not match
{
    "message": "unsuccessfully",
    "status": false,
    "count": 1,
    "results": "Username is already registered"
}

#response if password does not match
{
    "message": "unsuccessfully",
    "status": false,
    "count": 1,
    "results": "Password Minimum 8 Character"
}

#response if username has been registered
{
    "message": "unsuccessfully",
    "status": false,
    "count": 1,
    "results": "Username is already registered"
}

#response if email has been registered
{
    "message": "unsuccessfully",
    "status": false,
    "count": 1,
    "results": "Email is already registered"
}
````
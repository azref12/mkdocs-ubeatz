## Sign In by Google 

### Endpoint
````
[GET] url/user/email/?email=(confidential data) 
````

### GET Method
Use *email*  as ``params`` for sign in by google.

### Result 
````
{
    "message": "successfully",
    "status": true,
    "count": 1,
    "results": {
        "status": 9,
        "username": "(confidential data)",
        "id": (confidential data),
        "email": "(confidential data)",
        "details": [
            {
                "id": (confidential data),
                "reward": 0,
                "point": 65,
                "coin": 40,
                "phone_number": "(confidential data)",
                "pin": "(confidential data)",
                "code": (confidential data),
                "status": 1,
                "count_referal": 0,
                "idgetplus": "0",
                "membergetplus": "0",
                "extradata": null,
                "iduser_id": [
                    {
                        "id_up": (confidential data),
                        "id": (confidential data),
                        "profile": "media/profile/user.png"
                    }
                ]
            }
        ]
    }
}
````
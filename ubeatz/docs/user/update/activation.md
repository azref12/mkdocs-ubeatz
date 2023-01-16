## Activation Account 

### Endpoint
````
[GET] url/user/getactivation/?user=(confidential data)
````
````
[PUT] url/user/activation/ 
````

### GET Method 
For *GET* method, use *user* as ``params``.

### PUT Method
For *PUT* method, use this ``json`` file with the format below to activation account.
````
{
    "username": "(confidential data)",
    "codeuser": "(confidential data)",
    "phone_number": "(confidential data)"
}
````

### Result GET Method
````
{
    "message": "successfully",
    "status": true,
    "count": 1,
    "results": {
        "master": [
            {
                "id": (confidential data),
                "phone_number": "(confidential data)",
                "code": (confidential data),
                "status": 0
            }
        ],
        "detail": [
            {
                "id": (confidential data),
                "username": "(confidential data)",
                "email": "(confidential data)",
                "is_active": true
            }
        ]
    }
}
````
### Result PUT Method
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
                "status": 1,
                "count_referal": 0,
                "idgetplus": "0",
                "membergetplus": "0",
                "extradata": null
            }
        ],
        "message_refferal": false
    }
}
````
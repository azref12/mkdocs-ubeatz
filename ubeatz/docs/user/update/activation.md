## Activation Account 

### Endpoint
````
[GET] url/user/getactivation/?user=anonim12
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
    "username": "anonim12",
    "codeuser": "3920",
    "phone_number": "+6281234567891"
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
                "id": 2,
                "phone_number": "+6281234567891",
                "code": 4420,
                "status": 0
            }
        ],
        "detail": [
            {
                "id": 2,
                "username": "anonim12",
                "email": "anonim12@gmail.com",
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
                "id": 2,
                "reward": 0,
                "point": 0,
                "coin": 0,
                "phone_number": "+6281234567891",
                "pin": "JLN8WO",
                "code": 3920,
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
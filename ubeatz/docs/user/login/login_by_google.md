## Sign In by Google 

Endpoint
````
[GET] url/user/email/?email=anonim12@gmail.com 
````

## GET Method
Use ``email`` as ``params`` for sign in by google.

## Result 
````
{
    "message": "successfully",
    "status": true,
    "count": 1,
    "results": {
        "status": 9,
        "username": "anonim12",
        "id": 2,
        "email": "anonim12@gmail.com",
        "details": [
            {
                "id": 2,
                "reward": 0,
                "point": 65,
                "coin": 40,
                "phone_number": "+6281234567891",
                "pin": "JLN8WO",
                "code": 3920,
                "status": 1,
                "count_referal": 0,
                "idgetplus": "0",
                "membergetplus": "0",
                "extradata": null,
                "iduser_id": [
                    {
                        "id_up": 1,
                        "id": 2,
                        "profile": "media/profile/user.png"
                    }
                ]
            }
        ]
    }
}
````
## Sign In
Endpoint
````
    url/user/login [POST]
````
use this ``json`` file with the format below to sign in
````
{
    "username": "anonim12",
    "password": "123123123"
}
````
## Result
```` 
{
    "refresh": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJ0b2tlbl90eXBlIjoicmVmcmVzaCIsImV4cCI6MTY3MTg2OTU3NCwianRpIjoiNTRmMDAyOTA2ODkzNGRiMmE1YjM5YjRkYzEwZTdjYjEiLCJ1c2VyX2lkIjoyfQ.yz6zHw7gHud2qPvt-rHzqzTFiSvP71N4uhfhm1IzsCw",
    "access": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiZXhwIjoxNjcxNzgzNDc0LCJqdGkiOiJjNmU5ZDkwMzQxOGQ0YzYyOGQ3YTdjZDU1NTYzZTk0YSIsInVzZXJfaWQiOjJ9.QVEYvsmdbOgF1vlapuHsID07J_raYy_bmZU-Qi6OPnk",
    "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiZXhwIjoxNjcyNjQ3MTc0LCJqdGkiOiIyMDI1NDZkNjA5NzY0NWUxOWU2ZTg0MjY2OTZhYzM2NSIsInVzZXJfaWQiOjJ9.QIi_-6A7QoNBvFQKU_ALJN3yTebe7ED6YwRebvUb_E8",
    "username": "anonim12",
    "is_superuser": false,
    "is_staff": false,
    "id": 2,
    "firstName": "-",
    "lastName": "-",
    "email": "anonim12@gmail.com",
    "password": "pbkdf2_sha256$260000$mY0q9uMsBOv1c2YalSlucT$jWl1dq9nSw+erRuqCQp1b/TIwJNl/+9hX06qFbPCCXo=",
    "is_active": true,
    "details": [
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
            "extradata": null,
            "iduser_id": [
                {
                    "id_up": 1,
                    "id": 2,
                    "profile": "media/profile/default.png"
                }
            ]
        }
    ]
}
````
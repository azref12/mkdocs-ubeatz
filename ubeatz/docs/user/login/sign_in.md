## Sign In

### Endpoint
````
[POST] url/user/login 
````

### POST Method 
Use this ``json`` file with the format below to sign in.
````
{
    "username": "(confidential data)",
    "password": "(confidential data)"
}
````
### Result
```` 
{
    "refresh": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJ0b2tlbl90eXBlIjoicmVmcmVzaCIsImV4cCI6MTY3MTg2OTU3NCwianRpIjoiNTRmMDAyOTA2ODkzNGRiMmE1YjM5YjRkYzEwZTdjYjEiLCJ1c2VyX2lkIjoyfQ.yz6zHw7gHud2qPvt-rHzqzTFiSvP71N4uhfhm1IzsCw",
    "access": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiZXhwIjoxNjcxNzgzNDc0LCJqdGkiOiJjNmU5ZDkwMzQxOGQ0YzYyOGQ3YTdjZDU1NTYzZTk0YSIsInVzZXJfaWQiOjJ9.QVEYvsmdbOgF1vlapuHsID07J_raYy_bmZU-Qi6OPnk",
    "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiZXhwIjoxNjcyNjQ3MTc0LCJqdGkiOiIyMDI1NDZkNjA5NzY0NWUxOWU2ZTg0MjY2OTZhYzM2NSIsInVzZXJfaWQiOjJ9.QIi_-6A7QoNBvFQKU_ALJN3yTebe7ED6YwRebvUb_E8",
    "username": "(confidential data)",
    "is_superuser": false,
    "is_staff": false,
    "id": (confidential data),
    "firstName": "-",
    "lastName": "-",
    "email": "(confidential data)",
    "password": "pbkdf2_sha256$260000$mY0q9uMsBOv1c2YalSlucT$jWl1dq9nSw+erRuqCQp1b/TIwJNl/+9hX06qFbPCCXo=",
    "is_active": true,
    "details": [
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
````
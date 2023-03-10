## Add Point

### Endpoint
````
[POST] url/add_point/auth/ 
````
Before adding points, make sure you already have an account, ``username``  and ``password`` will be used as ``basic authentication`` to add points. On postman select ``authorization`` next to ``params``, then select ``basic auth type``, then insert the username and password that were registered previously.

![basic_auth_images](basic_auth.png)

### POST Method
Use this ``json`` file with the format below to add point.
````
{
    "email" : "(confidential data)",
    "userid" : (confidential data),
    "value_point" : 60
}
````
### Result
````
{
    "Status": true,
    "message": "added point successfully",
    "results": {
        "master": [
            {
                "id_addpoint": (confidential data),
                "value_point": 60,
                "email": "(confidential data)",
                "userid": (confidential data),
                "created_at": "2022-12-28T08:09:22.057864"
            }
        ]
    }
}
````
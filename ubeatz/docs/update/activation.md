## Account Activation
Endpoint
````
    url/user/activation/ [PUT]
````
use the json file with the format below to account activation
````
{
    "username": "anonim12",
    "codeuser": "3920",
    "phone_number": "+6281234567892"
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
                "phone_number": "+6281234567892",
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
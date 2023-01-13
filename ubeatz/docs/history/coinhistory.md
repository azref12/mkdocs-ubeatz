## Coin History 

### Endpoint
````
[GET] url/history/coin/?id=2 
````

### GET Method
For *GET* method, use *id* as ``params`` to get coin history.

### Result
````
{
    "message": "successfully",
    "results": {
        "coin": [
            {
                "id": 1,
                "transaksi": "(confidential data)",
                "coin": 40,
                "datehistory": "2022-12-27T07:10:58.683541",
                "status": 0,
                "statushistory": 1,
                "iduser": 2,
                "keterangan": "REDEM QWERTY12"
            }
        ],
        "details": [
            {
                "id": 2,
                "reward": 0,
                "point": 185,
                "coin": 40,
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

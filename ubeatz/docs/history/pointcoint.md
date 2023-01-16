## Point-Coin History 

### Endpoint
````
[GET] url/history/point-coint/?id=(confidential data) 
````

### GET Method
For *GET* method, use *id* as ``params`` to get point-coin history.

### Result
````
{
    "message": "successfully",
    "results": {
        "point": [
            {
                "id": (confidential data),
                "transaksi": "(confidential data)",
                "point": 40,
                "datehistory": "2022-12-26T12:36:29.494899",
                "status": 0,
                "statushistory": 1,
                "iduser": (confidential data),
                "keterangan": "REDEM QWERTY12"
            },
            {
                "id": (confidential data),
                "transaksi": "(confidential data)",
                "point": 250,
                "datehistory": "2022-12-26T12:39:57.273647",
                "status": 0,
                "statushistory": 1,
                "iduser": (confidential data),
                "keterangan": "REDEEM FOR NEW ACCOUNT, POINT SEND TO GETPLUS"
            },
            {
                "id": (confidential data),
                "transaksi": "(confidential data)",
                "point": 25,
                "datehistory": "2022-12-26T12:42:53.218745",
                "status": 0,
                "statushistory": 1,
                "iduser": (confidential data),
                "keterangan": "POINT FROM FEEDBACK"
            }
        ],
        "coin": [
            {
                "id": (confidential data),
                "transaksi": "(confidential data)",
                "coin": 40,
                "datehistory": "2022-12-26T12:36:29.510899",
                "status": 0,
                "statushistory": 1,
                "iduser": (confidential data),
                "keterangan": "REDEM QWERTY12"
            }
        ],
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
                "extradata": null
            }
        ]
    }
}
````
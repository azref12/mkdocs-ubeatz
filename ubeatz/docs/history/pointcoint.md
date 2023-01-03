## Point-Coin History 

Endpoint
````
[GET] url/history/point-coint/?id=2 
````

Use ``id`` as ``params`` to get point-coin history

## Result
````
{
    "message": "successfully",
    "results": {
        "point": [
            {
                "id": 1,
                "transaksi": "PI2212260001",
                "point": 40,
                "datehistory": "2022-12-26T12:36:29.494899",
                "status": 0,
                "statushistory": 1,
                "iduser": 2,
                "keterangan": "REDEM QWERTY12"
            },
            {
                "id": 2,
                "transaksi": "PI2212260002",
                "point": 250,
                "datehistory": "2022-12-26T12:39:57.273647",
                "status": 0,
                "statushistory": 1,
                "iduser": 2,
                "keterangan": "REDEEM FOR NEW ACCOUNT, POINT SEND TO GETPLUS"
            },
            {
                "id": 4,
                "transaksi": "PI2212260004",
                "point": 25,
                "datehistory": "2022-12-26T12:42:53.218745",
                "status": 0,
                "statushistory": 1,
                "iduser": 2,
                "keterangan": "POINT FROM FEEDBACK"
            }
        ],
        "coin": [
            {
                "id": 1,
                "transaksi": "CI2212260001",
                "coin": 40,
                "datehistory": "2022-12-26T12:36:29.510899",
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
                "point": 65,
                "coin": 40,
                "phone_number": "+6281234567891",
                "pin": "JLN8WO",
                "code": 3920,
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
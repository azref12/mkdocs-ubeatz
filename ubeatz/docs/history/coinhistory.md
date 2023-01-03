## Coin History 

Endpoint
````
[GET] url/history/coin/?id=2 
````

Use ``id`` as ``params`` to get coin history

## Result
````
{
    "message": "successfully",
    "results": {
        "coin": [
            {
                "id": 1,
                "transaksi": "CI2212270001",
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
                "phone_number": "+6281234567892",
                "pin": "9PEG5D",
                "code": 4420,
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

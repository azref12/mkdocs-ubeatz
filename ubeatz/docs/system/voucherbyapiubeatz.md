## Voucher by API Ubeatz

### Endpoint
````
[POST] http://api.ubeatz.co.id/v1/voucher
````
````
[GET] http://api.ubeatz.co.id/v1/voucher
````

### POST Method
Use this ``json`` file with the format below to insert voucher.
````
{
    "title": "test02",
    "code": "(confidential data)",
    "description": "Lorem Ipsum",
    "value": 100,
    "max_value": 100,
    "value_type": "price",
    "start_date": "2023-01-07T07:21:19.000+07:00",
    "expired_date": "2023-01-08T07:21:19.000+07:00",
    "quantity": 1,
    "actor": "ids"
}
````

### Result POST Method
````
{
    "meta": {
        "status": 201,
        "message": "Create voucher success"
    },
    "data": {
        "id": (confidential data),
        "title": "test02",
        "code": "(confidential data)",
        "description": "Lorem Ipsum",
        "value": 100,
        "max_value": 100,
        "value_type": "price",
        "voucher_type": "discount",
        "start_date": "2023-01-07T07:21:19.000+07:00",
        "expired_date": "2023-01-08T07:21:19.000+07:00",
        "quantity": 1,
        "created_at": "2023-01-09T15:28:27.000+07:00",
        "updated_at": "2023-01-09T15:28:27.000+07:00",
        "is_enable": true,
        "actor": "promotion",
        "status": "pending",
        "branches": [
            {
                "id": (confidential data),
                "voucher_id": (confidential data),
                "branch_id": (confidential data),
                "created_at": "2023-01-09T15:28:27.000+07:00",
                "updated_at": "2023-01-09T15:28:27.000+07:00",
                "name": "Summarecon Mall Serpong"
            },
            ...
        ]
    }
}
````

### Result GET Method
````
{
    "meta": {
        "status": 200,
        "message": "Fetch data success"
    },
    "data": [
        {
            "id": (confidential data)
            "title": "VCTEST80",
            "code": "(confidential data)",
            "description": "Voucher testing 80%",
            "value": 80,
            "max_value": 75000,
            "value_type": "percent",
            "voucher_type": "discount",
            "start_date": "2022-11-04T10:00:00.000+07:00",
            "expired_date": "2022-11-05T10:00:00.000+07:00",
            "quantity": 5,
            "created_at": "2022-11-04T09:48:54.000+07:00",
            "updated_at": "2022-11-04T09:48:54.000+07:00",
            "is_enable": true,
            "actor": "promotion",
            "status": "pending",
            "branches": [
                {
                    "id": (confidential data),
                    "voucher_id": (confidential data)
                    "branch_id": (confidential data),
                    "created_at": "2022-11-27T14:41:55.000+07:00",
                    "updated_at": "2022-11-27T14:41:55.000+07:00",
                    "name": "Posbloc"
                }
            ]
        },
        ...
    ]
}
````
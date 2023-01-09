## Voucher by API Ubeatz

Endpoint
````
[POST] http://api.ubeatz.co.id/v1/voucher
````
````
[GET] http://api.ubeatz.co.id/v1/voucher
````

## POST Method
Use this ``json`` file with the format below to insert voucher.
````
{
    "title": "test02",
    "code": "InDos0ft2023",
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

## Result POST Method
````
{
    "meta": {
        "status": 201,
        "message": "Create voucher success"
    },
    "data": {
        "id": 362,
        "title": "test02",
        "code": "InDos0ft2023",
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
                "id": 2429,
                "voucher_id": 362,
                "branch_id": 1,
                "created_at": "2023-01-09T15:28:27.000+07:00",
                "updated_at": "2023-01-09T15:28:27.000+07:00",
                "name": "Summarecon Mall Serpong"
            },
            {
                "id": 2430,
                "voucher_id": 362,
                "branch_id": 2,
                "created_at": "2023-01-09T15:28:27.000+07:00",
                "updated_at": "2023-01-09T15:28:27.000+07:00",
                "name": "Startspace Gading Serpong"
            },
            {
                "id": 2431,
                "voucher_id": 362,
                "branch_id": 3,
                "created_at": "2023-01-09T15:28:27.000+07:00",
                "updated_at": "2023-01-09T15:28:27.000+07:00",
                "name": "Posbloc"
            },
            {
                "id": 2432,
                "voucher_id": 362,
                "branch_id": 5,
                "created_at": "2023-01-09T15:28:27.000+07:00",
                "updated_at": "2023-01-09T15:28:27.000+07:00",
                "name": "Kantor Alsut"
            },
            {
                "id": 2433,
                "voucher_id": 362,
                "branch_id": 6,
                "created_at": "2023-01-09T15:28:27.000+07:00",
                "updated_at": "2023-01-09T15:28:27.000+07:00",
                "name": "Singkawang Grand Mall"
            },
            {
                "id": 2434,
                "voucher_id": 362,
                "branch_id": 7,
                "created_at": "2023-01-09T15:28:27.000+07:00",
                "updated_at": "2023-01-09T15:28:27.000+07:00",
                "name": "Summarecon"
            },
            {
                "id": 2435,
                "voucher_id": 362,
                "branch_id": 8,
                "created_at": "2023-01-09T15:28:27.000+07:00",
                "updated_at": "2023-01-09T15:28:27.000+07:00",
                "name": "Blok M Plaza"
            }
        ]
    }
}
````

## Result GET Method
````
{
    "meta": {
        "status": 200,
        "message": "Fetch data success"
    },
    "data": [
        {
            "id": 2,
            "title": "VCTEST80",
            "code": "VCTEST80",
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
                    "id": 256,
                    "voucher_id": 2,
                    "branch_id": 3,
                    "created_at": "2022-11-27T14:41:55.000+07:00",
                    "updated_at": "2022-11-27T14:41:55.000+07:00",
                    "name": "Posbloc"
                }
            ]
        },
        {
            "id": 3,
            "title": "VCTEST90",
            "code": "VCTEST90",
            "description": "Voucher test 90%",
            "value": 90,
            "max_value": 200000,
            "value_type": "percent",
            "voucher_type": "discount",
            "start_date": "2022-12-31T10:00:00.000+07:00",
            "expired_date": "2023-01-03T15:00:00.000+07:00",
            "quantity": 1,
            "created_at": "2022-11-04T10:37:11.000+07:00",
            "updated_at": "2022-12-31T13:34:26.000+07:00",
            "is_enable": true,
            "actor": "promotion",
            "status": "pending",
            "branches": [
                {
                    "id": 1257,
                    "voucher_id": 3,
                    "branch_id": 1,
                    "created_at": "2022-12-31T08:59:05.000+07:00",
                    "updated_at": "2022-12-31T08:59:05.000+07:00",
                    "name": "Summarecon Mall Serpong"
                },
                {
                    "id": 1258,
                    "voucher_id": 3,
                    "branch_id": 3,
                    "created_at": "2022-12-31T08:59:05.000+07:00",
                    "updated_at": "2022-12-31T08:59:05.000+07:00",
                    "name": "Posbloc"
                },
                {
                    "id": 1259,
                    "voucher_id": 3,
                    "branch_id": 8,
                    "created_at": "2022-12-31T08:59:05.000+07:00",
                    "updated_at": "2022-12-31T08:59:05.000+07:00",
                    "name": "Blok M Plaza"
                }
            ]
        },
        {
            "id": 4,
            "title": "Test vcode",
            "code": "VCTEST95",
            "description": "Voucher test 95%",
            "value": 95,
            "max_value": 2000000,
            "value_type": "percent",
            "voucher_type": "discount",
            "start_date": "2022-12-02T13:00:00.000+07:00",
            "expired_date": "2022-12-05T14:00:00.000+07:00",
            "quantity": 5,
            "created_at": "2022-11-09T14:27:55.000+07:00",
            "updated_at": "2022-12-02T19:02:19.000+07:00",
            "is_enable": true,
            "actor": "promotion",
            "status": "pending",
            "branches": [
                {
                    "id": 299,
                    "voucher_id": 4,
                    "branch_id": 1,
                    "created_at": "2022-12-02T12:49:58.000+07:00",
                    "updated_at": "2022-12-02T12:49:58.000+07:00",
                    "name": "Summarecon Mall Serpong"
                },
                {
                    "id": 300,
                    "voucher_id": 4,
                    "branch_id": 3,
                    "created_at": "2022-12-02T12:49:58.000+07:00",
                    "updated_at": "2022-12-02T12:49:58.000+07:00",
                    "name": "Posbloc"
                }
            ]
        },
        {
            "id": 6,
            "title": "Voucher F&B 20.000",
            "code": "AFWJ1234",
            "description": "Voucher F&B 20.000",
            "value": 90000,
            "max_value": 90000,
            "value_type": "price",
            "voucher_type": "discount",
            "start_date": "2022-11-14T10:35:14.000+07:00",
            "expired_date": "2022-11-21T00:00:00.000+07:00",
            "quantity": 1,
            "created_at": "2022-11-14T17:35:15.000+07:00",
            "updated_at": "2022-11-14T17:35:15.000+07:00",
            "is_enable": true,
            "actor": "promotion",
            "status": "pending",
            "branches": [
                {
                    "id": 58,
                    "voucher_id": 6,
                    "branch_id": 1,
                    "created_at": "2022-11-14T17:35:15.000+07:00",
                    "updated_at": "2022-11-14T17:35:15.000+07:00",
                    "name": "Summarecon Mall Serpong"
                },
                {
                    "id": 59,
                    "voucher_id": 6,
                    "branch_id": 2,
                    "created_at": "2022-11-14T17:35:15.000+07:00",
                    "updated_at": "2022-11-14T17:35:15.000+07:00",
                    "name": "Startspace Gading Serpong"
                },
                {
                    "id": 60,
                    "voucher_id": 6,
                    "branch_id": 3,
                    "created_at": "2022-11-14T17:35:15.000+07:00",
                    "updated_at": "2022-11-14T17:35:15.000+07:00",
                    "name": "Posbloc"
                },
                {
                    "id": 61,
                    "voucher_id": 6,
                    "branch_id": 5,
                    "created_at": "2022-11-14T17:35:15.000+07:00",
                    "updated_at": "2022-11-14T17:35:15.000+07:00",
                    "name": "Kantor Alsut"
                },
                {
                    "id": 62,
                    "voucher_id": 6,
                    "branch_id": 6,
                    "created_at": "2022-11-14T17:35:15.000+07:00",
                    "updated_at": "2022-11-14T17:35:15.000+07:00",
                    "name": "Singkawang Grand Mall"
                },
                {
                    "id": 63,
                    "voucher_id": 6,
                    "branch_id": 7,
                    "created_at": "2022-11-14T17:35:15.000+07:00",
                    "updated_at": "2022-11-14T17:35:15.000+07:00",
                    "name": "Summarecon"
                }
            ]
        },
        {
            "id": 7,
            "title": "Voucher F&B 25.000",
            "code": "YYRT4321",
            "description": "no terms and conditions",
            "value": 25000,
            "max_value": 25000,
            "value_type": "price",
            "voucher_type": "discount",
            "start_date": "2022-11-14T11:08:15.000+07:00",
            "expired_date": "2022-11-21T00:00:00.000+07:00",
            "quantity": 1,
            "created_at": "2022-11-14T18:08:16.000+07:00",
            "updated_at": "2022-11-14T18:08:16.000+07:00",
            "is_enable": true,
            "actor": "promotion",
            "status": "pending",
            "branches": [
                {
                    "id": 64,
                    "voucher_id": 7,
                    "branch_id": 1,
                    "created_at": "2022-11-14T18:08:16.000+07:00",
                    "updated_at": "2022-11-14T18:08:16.000+07:00",
                    "name": "Summarecon Mall Serpong"
                },
                {
                    "id": 65,
                    "voucher_id": 7,
                    "branch_id": 2,
                    "created_at": "2022-11-14T18:08:16.000+07:00",
                    "updated_at": "2022-11-14T18:08:16.000+07:00",
                    "name": "Startspace Gading Serpong"
                },
                {
                    "id": 66,
                    "voucher_id": 7,
                    "branch_id": 3,
                    "created_at": "2022-11-14T18:08:16.000+07:00",
                    "updated_at": "2022-11-14T18:08:16.000+07:00",
                    "name": "Posbloc"
                },
                {
                    "id": 67,
                    "voucher_id": 7,
                    "branch_id": 5,
                    "created_at": "2022-11-14T18:08:16.000+07:00",
                    "updated_at": "2022-11-14T18:08:16.000+07:00",
                    "name": "Kantor Alsut"
                },
                {
                    "id": 68,
                    "voucher_id": 7,
                    "branch_id": 6,
                    "created_at": "2022-11-14T18:08:16.000+07:00",
                    "updated_at": "2022-11-14T18:08:16.000+07:00",
                    "name": "Singkawang Grand Mall"
                },
                {
                    "id": 69,
                    "voucher_id": 7,
                    "branch_id": 7,
                    "created_at": "2022-11-14T18:08:16.000+07:00",
                    "updated_at": "2022-11-14T18:08:16.000+07:00",
                    "name": "Summarecon"
                }
            ]
        },
        {
            "id": 8,
            "title": "Voucher F&B 20.000",
            "code": "IUYT8421",
            "description": "S&K. minimum pembelanjaan 50ribu dan wajib purchase durasi waktu minimal 30 menit",
            "value": 90000,
            "max_value": 90000,
            "value_type": "price",
            "voucher_type": "discount",
            "start_date": "2022-11-15T05:38:49.000+07:00",
            "expired_date": "2022-11-22T00:00:00.000+07:00",
            "quantity": 1,
            "created_at": "2022-11-15T12:38:49.000+07:00",
            "updated_at": "2022-11-15T12:38:49.000+07:00",
            "is_enable": true,
            "actor": "promotion",
            "status": "pending",
            "branches": [
                {
                    "id": 1230,
                    "voucher_id": 8,
                    "branch_id": 1,
                    "created_at": "2022-12-30T17:12:58.000+07:00",
                    "updated_at": "2022-12-30T17:12:58.000+07:00",
                    "name": "Summarecon Mall Serpong"
                },
                {
                    "id": 1231,
                    "voucher_id": 8,
                    "branch_id": 2,
                    "created_at": "2022-12-30T17:12:58.000+07:00",
                    "updated_at": "2022-12-30T17:12:58.000+07:00",
                    "name": "Startspace Gading Serpong"
                },
                {
                    "id": 1232,
                    "voucher_id": 8,
                    "branch_id": 3,
                    "created_at": "2022-12-30T17:12:58.000+07:00",
                    "updated_at": "2022-12-30T17:12:58.000+07:00",
                    "name": "Posbloc"
                },
                {
                    "id": 1233,
                    "voucher_id": 8,
                    "branch_id": 5,
                    "created_at": "2022-12-30T17:12:58.000+07:00",
                    "updated_at": "2022-12-30T17:12:58.000+07:00",
                    "name": "Kantor Alsut"
                },
                {
                    "id": 1234,
                    "voucher_id": 8,
                    "branch_id": 6,
                    "created_at": "2022-12-30T17:12:58.000+07:00",
                    "updated_at": "2022-12-30T17:12:58.000+07:00",
                    "name": "Singkawang Grand Mall"
                },
                {
                    "id": 1235,
                    "voucher_id": 8,
                    "branch_id": 7,
                    "created_at": "2022-12-30T17:12:58.000+07:00",
                    "updated_at": "2022-12-30T17:12:58.000+07:00",
                    "name": "Summarecon"
                }
            ]
        },
        {
            "id": 12,
            "title": "Voucher 10 Menit Free",
            "code": "BVCX4315",
            "description": "S&K. minimum pembelanjaan 50ribu dan wajib purchase durasi waktu minimal 30 menit",
            "value": 0,
            "max_value": 0,
            "value_type": "price",
            "voucher_type": "discount",
            "start_date": "2022-11-16T12:20:51.000+07:00",
            "expired_date": "2022-11-23T00:00:00.000+07:00",
            "quantity": 1,
            "created_at": "2022-11-16T19:20:51.000+07:00",
            "updated_at": "2022-11-16T19:20:51.000+07:00",
            "is_enable": true,
            "actor": "promotion",
            "status": "pending",
            "branches": [
                {
                    "id": 94,
                    "voucher_id": 12,
                    "branch_id": 1,
                    "created_at": "2022-11-16T19:20:51.000+07:00",
                    "updated_at": "2022-11-16T19:20:51.000+07:00",
                    "name": "Summarecon Mall Serpong"
                },
                {
                    "id": 95,
                    "voucher_id": 12,
                    "branch_id": 2,
                    "created_at": "2022-11-16T19:20:51.000+07:00",
                    "updated_at": "2022-11-16T19:20:51.000+07:00",
                    "name": "Startspace Gading Serpong"
                },
                {
                    "id": 96,
                    "voucher_id": 12,
                    "branch_id": 3,
                    "created_at": "2022-11-16T19:20:51.000+07:00",
                    "updated_at": "2022-11-16T19:20:51.000+07:00",
                    "name": "Posbloc"
                },
                {
                    "id": 97,
                    "voucher_id": 12,
                    "branch_id": 5,
                    "created_at": "2022-11-16T19:20:51.000+07:00",
                    "updated_at": "2022-11-16T19:20:51.000+07:00",
                    "name": "Kantor Alsut"
                },
                {
                    "id": 98,
                    "voucher_id": 12,
                    "branch_id": 6,
                    "created_at": "2022-11-16T19:20:51.000+07:00",
                    "updated_at": "2022-11-16T19:20:51.000+07:00",
                    "name": "Singkawang Grand Mall"
                },
                {
                    "id": 99,
                    "voucher_id": 12,
                    "branch_id": 7,
                    "created_at": "2022-11-16T19:20:51.000+07:00",
                    "updated_at": "2022-11-16T19:20:51.000+07:00",
                    "name": "Summarecon"
                }
            ]
        },
        {
            "id": 13,
            "title": "Voucher 10 Menit Free",
            "code": "MNBV4321",
            "description": "S&K. minimum pembelanjaan 50ribu dan wajib purchase durasi waktu minimal 30 menit",
            "value": 0,
            "max_value": 0,
            "value_type": "price",
            "voucher_type": "discount",
            "start_date": "2022-11-17T05:46:04.000+07:00",
            "expired_date": "2022-11-24T00:00:00.000+07:00",
            "quantity": 1,
            "created_at": "2022-11-17T12:46:04.000+07:00",
            "updated_at": "2022-11-17T12:46:04.000+07:00",
            "is_enable": true,
            "actor": "promotion",
            "status": "active",
            "branches": [
                {
                    "id": 106,
                    "voucher_id": 13,
                    "branch_id": 1,
                    "created_at": "2022-11-17T12:46:04.000+07:00",
                    "updated_at": "2022-11-17T12:46:04.000+07:00",
                    "name": "Summarecon Mall Serpong"
                },
                {
                    "id": 107,
                    "voucher_id": 13,
                    "branch_id": 2,
                    "created_at": "2022-11-17T12:46:04.000+07:00",
                    "updated_at": "2022-11-17T12:46:04.000+07:00",
                    "name": "Startspace Gading Serpong"
                },
                {
                    "id": 108,
                    "voucher_id": 13,
                    "branch_id": 3,
                    "created_at": "2022-11-17T12:46:04.000+07:00",
                    "updated_at": "2022-11-17T12:46:04.000+07:00",
                    "name": "Posbloc"
                },
                {
                    "id": 109,
                    "voucher_id": 13,
                    "branch_id": 5,
                    "created_at": "2022-11-17T12:46:04.000+07:00",
                    "updated_at": "2022-11-17T12:46:04.000+07:00",
                    "name": "Kantor Alsut"
                },
                {
                    "id": 110,
                    "voucher_id": 13,
                    "branch_id": 6,
                    "created_at": "2022-11-17T12:46:04.000+07:00",
                    "updated_at": "2022-11-17T12:46:04.000+07:00",
                    "name": "Singkawang Grand Mall"
                },
                {
                    "id": 111,
                    "voucher_id": 13,
                    "branch_id": 7,
                    "created_at": "2022-11-17T12:46:04.000+07:00",
                    "updated_at": "2022-11-17T12:46:04.000+07:00",
                    "name": "Summarecon"
                }
            ]
        },
        {
            "id": 14,
            "title": "Voucher F&B 25.000",
            "code": "AEZ4KM10",
            "description": "no terms and conditions",
            "value": 25000,
            "max_value": 25000,
            "value_type": "price",
            "voucher_type": "discount",
            "start_date": "2022-11-17T06:53:59.000+07:00",
            "expired_date": "2022-11-24T00:00:00.000+07:00",
            "quantity": 1,
            "created_at": "2022-11-17T13:53:59.000+07:00",
            "updated_at": "2022-11-17T13:53:59.000+07:00",
            "is_enable": true,
            "actor": "promotion",
            "status": "pending",
            "branches": [
                {
                    "id": 112,
                    "voucher_id": 14,
                    "branch_id": 1,
                    "created_at": "2022-11-17T13:53:59.000+07:00",
                    "updated_at": "2022-11-17T13:53:59.000+07:00",
                    "name": "Summarecon Mall Serpong"
                },
                {
                    "id": 113,
                    "voucher_id": 14,
                    "branch_id": 2,
                    "created_at": "2022-11-17T13:53:59.000+07:00",
                    "updated_at": "2022-11-17T13:53:59.000+07:00",
                    "name": "Startspace Gading Serpong"
                },
                {
                    "id": 114,
                    "voucher_id": 14,
                    "branch_id": 3,
                    "created_at": "2022-11-17T13:53:59.000+07:00",
                    "updated_at": "2022-11-17T13:53:59.000+07:00",
                    "name": "Posbloc"
                },
                {
                    "id": 115,
                    "voucher_id": 14,
                    "branch_id": 5,
                    "created_at": "2022-11-17T13:53:59.000+07:00",
                    "updated_at": "2022-11-17T13:53:59.000+07:00",
                    "name": "Kantor Alsut"
                },
                {
                    "id": 116,
                    "voucher_id": 14,
                    "branch_id": 6,
                    "created_at": "2022-11-17T13:53:59.000+07:00",
                    "updated_at": "2022-11-17T13:53:59.000+07:00",
                    "name": "Singkawang Grand Mall"
                },
                {
                    "id": 117,
                    "voucher_id": 14,
                    "branch_id": 7,
                    "created_at": "2022-11-17T13:53:59.000+07:00",
                    "updated_at": "2022-11-17T13:53:59.000+07:00",
                    "name": "Summarecon"
                }
            ]
        },
        {
            "id": 15,
            "title": "Voucher F&B 20.000",
            "code": "SFGH1234",
            "description": "S&K. minimum pembelanjaan 50ribu dan wajib purchase durasi waktu minimal 30 menit",
            "value": 90000,
            "max_value": 90000,
            "value_type": "price",
            "voucher_type": "discount",
            "start_date": "2022-11-17T09:57:54.000+07:00",
            "expired_date": "2022-11-24T00:00:00.000+07:00",
            "quantity": 1,
            "created_at": "2022-11-17T16:57:54.000+07:00",
            "updated_at": "2022-11-17T16:57:54.000+07:00",
            "is_enable": true,
            "actor": "promotion",
            "status": "pending",
            "branches": [
                {
                    "id": 118,
                    "voucher_id": 15,
                    "branch_id": 1,
                    "created_at": "2022-11-17T16:57:54.000+07:00",
                    "updated_at": "2022-11-17T16:57:54.000+07:00",
                    "name": "Summarecon Mall Serpong"
                },
                {
                    "id": 119,
                    "voucher_id": 15,
                    "branch_id": 2,
                    "created_at": "2022-11-17T16:57:54.000+07:00",
                    "updated_at": "2022-11-17T16:57:54.000+07:00",
                    "name": "Startspace Gading Serpong"
                },
                {
                    "id": 120,
                    "voucher_id": 15,
                    "branch_id": 3,
                    "created_at": "2022-11-17T16:57:54.000+07:00",
                    "updated_at": "2022-11-17T16:57:54.000+07:00",
                    "name": "Posbloc"
                },
                {
                    "id": 121,
                    "voucher_id": 15,
                    "branch_id": 5,
                    "created_at": "2022-11-17T16:57:54.000+07:00",
                    "updated_at": "2022-11-17T16:57:54.000+07:00",
                    "name": "Kantor Alsut"
                },
                {
                    "id": 122,
                    "voucher_id": 15,
                    "branch_id": 6,
                    "created_at": "2022-11-17T16:57:54.000+07:00",
                    "updated_at": "2022-11-17T16:57:54.000+07:00",
                    "name": "Singkawang Grand Mall"
                },
                {
                    "id": 123,
                    "voucher_id": 15,
                    "branch_id": 7,
                    "created_at": "2022-11-17T16:57:54.000+07:00",
                    "updated_at": "2022-11-17T16:57:54.000+07:00",
                    "name": "Summarecon"
                }
            ]
        },
        {
            "id": 16,
            "title": "Voucher 30 Menit Free",
            "code": "HRSE3214",
            "description": "no terms and conditions",
            "value": 90000,
            "max_value": 90000,
            "value_type": "price",
            "voucher_type": "discount",
            "start_date": "2022-11-17T10:21:05.000+07:00",
            "expired_date": "2022-11-24T00:00:00.000+07:00",
            "quantity": 1,
            "created_at": "2022-11-17T17:21:05.000+07:00",
            "updated_at": "2022-11-17T17:21:05.000+07:00",
            "is_enable": true,
            "actor": "promotion",
            "status": "pending",
            "branches": [
                {
                    "id": 124,
                    "voucher_id": 16,
                    "branch_id": 1,
                    "created_at": "2022-11-17T17:21:05.000+07:00",
                    "updated_at": "2022-11-17T17:21:05.000+07:00",
                    "name": "Summarecon Mall Serpong"
                },
                {
                    "id": 125,
                    "voucher_id": 16,
                    "branch_id": 2,
                    "created_at": "2022-11-17T17:21:05.000+07:00",
                    "updated_at": "2022-11-17T17:21:05.000+07:00",
                    "name": "Startspace Gading Serpong"
                },
                {
                    "id": 126,
                    "voucher_id": 16,
                    "branch_id": 3,
                    "created_at": "2022-11-17T17:21:05.000+07:00",
                    "updated_at": "2022-11-17T17:21:05.000+07:00",
                    "name": "Posbloc"
                },
                {
                    "id": 127,
                    "voucher_id": 16,
                    "branch_id": 5,
                    "created_at": "2022-11-17T17:21:05.000+07:00",
                    "updated_at": "2022-11-17T17:21:05.000+07:00",
                    "name": "Kantor Alsut"
                },
                {
                    "id": 128,
                    "voucher_id": 16,
                    "branch_id": 6,
                    "created_at": "2022-11-17T17:21:05.000+07:00",
                    "updated_at": "2022-11-17T17:21:05.000+07:00",
                    "name": "Singkawang Grand Mall"
                },
                {
                    "id": 129,
                    "voucher_id": 16,
                    "branch_id": 7,
                    "created_at": "2022-11-17T17:21:05.000+07:00",
                    "updated_at": "2022-11-17T17:21:05.000+07:00",
                    "name": "Summarecon"
                }
            ]
        },
        {
            "id": 17,
            "title": "Voucher 10 Menit Free",
            "code": "TEST0001",
            "description": "S&K. minimum pembelanjaan 50ribu dan wajib purchase durasi waktu minimal 30 menit",
            "value": 0,
            "max_value": 0,
            "value_type": "price",
            "voucher_type": "discount",
            "start_date": "2022-11-17T11:38:39.000+07:00",
            "expired_date": "2022-11-24T00:00:00.000+07:00",
            "quantity": 1,
            "created_at": "2022-11-17T18:38:39.000+07:00",
            "updated_at": "2022-11-17T18:38:39.000+07:00",
            "is_enable": true,
            "actor": "promotion",
            "status": "pending",
            "branches": [
                {
                    "id": 130,
                    "voucher_id": 17,
                    "branch_id": 1,
                    "created_at": "2022-11-17T18:38:39.000+07:00",
                    "updated_at": "2022-11-17T18:38:39.000+07:00",
                    "name": "Summarecon Mall Serpong"
                },
                {
                    "id": 131,
                    "voucher_id": 17,
                    "branch_id": 2,
                    "created_at": "2022-11-17T18:38:39.000+07:00",
                    "updated_at": "2022-11-17T18:38:39.000+07:00",
                    "name": "Startspace Gading Serpong"
                },
                {
                    "id": 132,
                    "voucher_id": 17,
                    "branch_id": 3,
                    "created_at": "2022-11-17T18:38:39.000+07:00",
                    "updated_at": "2022-11-17T18:38:39.000+07:00",
                    "name": "Posbloc"
                },
                {
                    "id": 133,
                    "voucher_id": 17,
                    "branch_id": 5,
                    "created_at": "2022-11-17T18:38:39.000+07:00",
                    "updated_at": "2022-11-17T18:38:39.000+07:00",
                    "name": "Kantor Alsut"
                },
                {
                    "id": 134,
                    "voucher_id": 17,
                    "branch_id": 6,
                    "created_at": "2022-11-17T18:38:39.000+07:00",
                    "updated_at": "2022-11-17T18:38:39.000+07:00",
                    "name": "Singkawang Grand Mall"
                },
                {
                    "id": 135,
                    "voucher_id": 17,
                    "branch_id": 7,
                    "created_at": "2022-11-17T18:38:39.000+07:00",
                    "updated_at": "2022-11-17T18:38:39.000+07:00",
                    "name": "Summarecon"
                }
            ]
        },
        {
            "id": 18,
            "title": "Voucher 10 Menit Free",
            "code": "TEST01",
            "description": "S&K. minimum pembelanjaan 50ribu dan wajib purchase durasi waktu minimal 30 menit",
            "value": 0,
            "max_value": 0,
            "value_type": "price",
            "voucher_type": "discount",
            "start_date": "2022-11-18T12:29:40.000+07:00",
            "expired_date": "2022-11-25T00:00:00.000+07:00",
            "quantity": 1,
            "created_at": "2022-11-18T19:29:48.000+07:00",
            "updated_at": "2022-11-18T19:29:48.000+07:00",
            "is_enable": true,
            "actor": "promotion",
            "status": "pending",
            "branches": [
                {
                    "id": 136,
                    "voucher_id": 18,
                    "branch_id": 1,
                    "created_at": "2022-11-18T19:29:48.000+07:00",
                    "updated_at": "2022-11-18T19:29:48.000+07:00",
                    "name": "Summarecon Mall Serpong"
                },
                {
                    "id": 137,
                    "voucher_id": 18,
                    "branch_id": 2,
                    "created_at": "2022-11-18T19:29:48.000+07:00",
                    "updated_at": "2022-11-18T19:29:48.000+07:00",
                    "name": "Startspace Gading Serpong"
                },
                {
                    "id": 138,
                    "voucher_id": 18,
                    "branch_id": 3,
                    "created_at": "2022-11-18T19:29:48.000+07:00",
                    "updated_at": "2022-11-18T19:29:48.000+07:00",
                    "name": "Posbloc"
                },
                {
                    "id": 139,
                    "voucher_id": 18,
                    "branch_id": 5,
                    "created_at": "2022-11-18T19:29:48.000+07:00",
                    "updated_at": "2022-11-18T19:29:48.000+07:00",
                    "name": "Kantor Alsut"
                },
                {
                    "id": 140,
                    "voucher_id": 18,
                    "branch_id": 6,
                    "created_at": "2022-11-18T19:29:48.000+07:00",
                    "updated_at": "2022-11-18T19:29:48.000+07:00",
                    "name": "Singkawang Grand Mall"
                },
                {
                    "id": 141,
                    "voucher_id": 18,
                    "branch_id": 7,
                    "created_at": "2022-11-18T19:29:48.000+07:00",
                    "updated_at": "2022-11-18T19:29:48.000+07:00",
                    "name": "Summarecon"
                }
            ]
        },
        {
            "id": 21,
            "title": "Voucher F&B 20.000",
            "code": "UFBRrbzGU",
            "description": "S&K. minimum pembelanjaan 50ribu dan wajib purchase durasi waktu minimal 30 menit",
            "value": 90000,
            "max_value": 90000,
            "value_type": "price",
            "voucher_type": "discount",
            "start_date": "2022-11-21T08:25:28.000+07:00",
            "expired_date": "2022-11-28T00:00:00.000+07:00",
            "quantity": 1,
            "created_at": "2022-11-21T15:25:36.000+07:00",
            "updated_at": "2022-11-21T15:25:36.000+07:00",
            "is_enable": true,
            "actor": "promotion",
            "status": "pending",
            "branches": [
                {
                    "id": 154,
                    "voucher_id": 21,
                    "branch_id": 1,
                    "created_at": "2022-11-21T15:25:36.000+07:00",
                    "updated_at": "2022-11-21T15:25:36.000+07:00",
                    "name": "Summarecon Mall Serpong"
                },
                {
                    "id": 155,
                    "voucher_id": 21,
                    "branch_id": 2,
                    "created_at": "2022-11-21T15:25:36.000+07:00",
                    "updated_at": "2022-11-21T15:25:36.000+07:00",
                    "name": "Startspace Gading Serpong"
                },
                {
                    "id": 156,
                    "voucher_id": 21,
                    "branch_id": 3,
                    "created_at": "2022-11-21T15:25:36.000+07:00",
                    "updated_at": "2022-11-21T15:25:36.000+07:00",
                    "name": "Posbloc"
                },
                {
                    "id": 157,
                    "voucher_id": 21,
                    "branch_id": 5,
                    "created_at": "2022-11-21T15:25:36.000+07:00",
                    "updated_at": "2022-11-21T15:25:36.000+07:00",
                    "name": "Kantor Alsut"
                },
                {
                    "id": 158,
                    "voucher_id": 21,
                    "branch_id": 6,
                    "created_at": "2022-11-21T15:25:36.000+07:00",
                    "updated_at": "2022-11-21T15:25:36.000+07:00",
                    "name": "Singkawang Grand Mall"
                },
                {
                    "id": 159,
                    "voucher_id": 21,
                    "branch_id": 7,
                    "created_at": "2022-11-21T15:25:36.000+07:00",
                    "updated_at": "2022-11-21T15:25:36.000+07:00",
                    "name": "Summarecon"
                }
            ]
        },
        {
            "id": 22,
            "title": "Voucher F&B 20.000",
            "code": "UFBcwqBPx",
            "description": "S&K. minimum pembelanjaan 50ribu dan wajib purchase durasi waktu minimal 30 menit",
            "value": 90000,
            "max_value": 90000,
            "value_type": "price",
            "voucher_type": "discount",
            "start_date": "2022-11-21T08:43:25.000+07:00",
            "expired_date": "2022-11-28T00:00:00.000+07:00",
            "quantity": 1,
            "created_at": "2022-11-21T15:43:34.000+07:00",
            "updated_at": "2022-11-21T15:43:34.000+07:00",
            "is_enable": true,
            "actor": "promotion",
            "status": "pending",
            "branches": [
                {
                    "id": 160,
                    "voucher_id": 22,
                    "branch_id": 1,
                    "created_at": "2022-11-21T15:43:34.000+07:00",
                    "updated_at": "2022-11-21T15:43:34.000+07:00",
                    "name": "Summarecon Mall Serpong"
                },
                {
                    "id": 161,
                    "voucher_id": 22,
                    "branch_id": 2,
                    "created_at": "2022-11-21T15:43:34.000+07:00",
                    "updated_at": "2022-11-21T15:43:34.000+07:00",
                    "name": "Startspace Gading Serpong"
                },
                {
                    "id": 162,
                    "voucher_id": 22,
                    "branch_id": 3,
                    "created_at": "2022-11-21T15:43:34.000+07:00",
                    "updated_at": "2022-11-21T15:43:34.000+07:00",
                    "name": "Posbloc"
                },
                {
                    "id": 163,
                    "voucher_id": 22,
                    "branch_id": 5,
                    "created_at": "2022-11-21T15:43:34.000+07:00",
                    "updated_at": "2022-11-21T15:43:34.000+07:00",
                    "name": "Kantor Alsut"
                },
                {
                    "id": 164,
                    "voucher_id": 22,
                    "branch_id": 6,
                    "created_at": "2022-11-21T15:43:34.000+07:00",
                    "updated_at": "2022-11-21T15:43:34.000+07:00",
                    "name": "Singkawang Grand Mall"
                },
                {
                    "id": 165,
                    "voucher_id": 22,
                    "branch_id": 7,
                    "created_at": "2022-11-21T15:43:34.000+07:00",
                    "updated_at": "2022-11-21T15:43:34.000+07:00",
                    "name": "Summarecon"
                }
            ]
        },
        {
            "id": 23,
            "title": "Voucher F&B 20.000",
            "code": "UFBhRykxc",
            "description": "S&K. minimum pembelanjaan 50ribu dan wajib purchase durasi waktu minimal 30 menit",
            "value": 90000,
            "max_value": 90000,
            "value_type": "price",
            "voucher_type": "discount",
            "start_date": "2022-11-21T09:27:19.000+07:00",
            "expired_date": "2022-11-28T00:00:00.000+07:00",
            "quantity": 1,
            "created_at": "2022-11-21T16:27:27.000+07:00",
            "updated_at": "2022-11-21T16:27:27.000+07:00",
            "is_enable": true,
            "actor": "promotion",
            "status": "pending",
            "branches": [
                {
                    "id": 166,
                    "voucher_id": 23,
                    "branch_id": 1,
                    "created_at": "2022-11-21T16:27:27.000+07:00",
                    "updated_at": "2022-11-21T16:27:27.000+07:00",
                    "name": "Summarecon Mall Serpong"
                },
                {
                    "id": 167,
                    "voucher_id": 23,
                    "branch_id": 2,
                    "created_at": "2022-11-21T16:27:27.000+07:00",
                    "updated_at": "2022-11-21T16:27:27.000+07:00",
                    "name": "Startspace Gading Serpong"
                },
                {
                    "id": 168,
                    "voucher_id": 23,
                    "branch_id": 3,
                    "created_at": "2022-11-21T16:27:27.000+07:00",
                    "updated_at": "2022-11-21T16:27:27.000+07:00",
                    "name": "Posbloc"
                },
                {
                    "id": 169,
                    "voucher_id": 23,
                    "branch_id": 5,
                    "created_at": "2022-11-21T16:27:27.000+07:00",
                    "updated_at": "2022-11-21T16:27:27.000+07:00",
                    "name": "Kantor Alsut"
                },
                {
                    "id": 170,
                    "voucher_id": 23,
                    "branch_id": 6,
                    "created_at": "2022-11-21T16:27:27.000+07:00",
                    "updated_at": "2022-11-21T16:27:27.000+07:00",
                    "name": "Singkawang Grand Mall"
                },
                {
                    "id": 171,
                    "voucher_id": 23,
                    "branch_id": 7,
                    "created_at": "2022-11-21T16:27:27.000+07:00",
                    "updated_at": "2022-11-21T16:27:27.000+07:00",
                    "name": "Summarecon"
                }
            ]
        },
        {
            "id": 24,
            "title": "Voucher F&B 20.000",
            "code": "UFBqHwz6C",
            "description": "S&K. minimum pembelanjaan 50ribu dan wajib purchase durasi waktu minimal 30 menit",
            "value": 90000,
            "max_value": 90000,
            "value_type": "price",
            "voucher_type": "discount",
            "start_date": "2022-11-21T10:27:45.000+07:00",
            "expired_date": "2022-11-28T00:00:00.000+07:00",
            "quantity": 1,
            "created_at": "2022-11-21T17:27:55.000+07:00",
            "updated_at": "2022-11-21T17:27:55.000+07:00",
            "is_enable": true,
            "actor": "promotion",
            "status": "pending",
            "branches": [
                {
                    "id": 172,
                    "voucher_id": 24,
                    "branch_id": 1,
                    "created_at": "2022-11-21T17:27:55.000+07:00",
                    "updated_at": "2022-11-21T17:27:55.000+07:00",
                    "name": "Summarecon Mall Serpong"
                },
                {
                    "id": 173,
                    "voucher_id": 24,
                    "branch_id": 2,
                    "created_at": "2022-11-21T17:27:55.000+07:00",
                    "updated_at": "2022-11-21T17:27:55.000+07:00",
                    "name": "Startspace Gading Serpong"
                },
                {
                    "id": 174,
                    "voucher_id": 24,
                    "branch_id": 3,
                    "created_at": "2022-11-21T17:27:55.000+07:00",
                    "updated_at": "2022-11-21T17:27:55.000+07:00",
                    "name": "Posbloc"
                },
                {
                    "id": 175,
                    "voucher_id": 24,
                    "branch_id": 5,
                    "created_at": "2022-11-21T17:27:55.000+07:00",
                    "updated_at": "2022-11-21T17:27:55.000+07:00",
                    "name": "Kantor Alsut"
                },
                {
                    "id": 176,
                    "voucher_id": 24,
                    "branch_id": 6,
                    "created_at": "2022-11-21T17:27:55.000+07:00",
                    "updated_at": "2022-11-21T17:27:55.000+07:00",
                    "name": "Singkawang Grand Mall"
                },
                {
                    "id": 177,
                    "voucher_id": 24,
                    "branch_id": 7,
                    "created_at": "2022-11-21T17:27:55.000+07:00",
                    "updated_at": "2022-11-21T17:27:55.000+07:00",
                    "name": "Summarecon"
                }
            ]
        },
        {
            "id": 25,
            "title": "Voucher F&B 20.000",
            "code": "UFBkKFLoB",
            "description": "S&K. minimum pembelanjaan 50ribu dan wajib purchase durasi waktu minimal 30 menit",
            "value": 90000,
            "max_value": 90000,
            "value_type": "price",
            "voucher_type": "discount",
            "start_date": "2022-11-22T03:10:23.000+07:00",
            "expired_date": "2022-11-29T00:00:00.000+07:00",
            "quantity": 1,
            "created_at": "2022-11-22T10:10:31.000+07:00",
            "updated_at": "2022-11-22T10:10:31.000+07:00",
            "is_enable": true,
            "actor": "promotion",
            "status": "pending",
            "branches": [
                {
                    "id": 178,
                    "voucher_id": 25,
                    "branch_id": 1,
                    "created_at": "2022-11-22T10:10:31.000+07:00",
                    "updated_at": "2022-11-22T10:10:31.000+07:00",
                    "name": "Summarecon Mall Serpong"
                },
                {
                    "id": 179,
                    "voucher_id": 25,
                    "branch_id": 2,
                    "created_at": "2022-11-22T10:10:31.000+07:00",
                    "updated_at": "2022-11-22T10:10:31.000+07:00",
                    "name": "Startspace Gading Serpong"
                },
                {
                    "id": 180,
                    "voucher_id": 25,
                    "branch_id": 3,
                    "created_at": "2022-11-22T10:10:31.000+07:00",
                    "updated_at": "2022-11-22T10:10:31.000+07:00",
                    "name": "Posbloc"
                },
                {
                    "id": 181,
                    "voucher_id": 25,
                    "branch_id": 5,
                    "created_at": "2022-11-22T10:10:31.000+07:00",
                    "updated_at": "2022-11-22T10:10:31.000+07:00",
                    "name": "Kantor Alsut"
                },
                {
                    "id": 182,
                    "voucher_id": 25,
                    "branch_id": 6,
                    "created_at": "2022-11-22T10:10:31.000+07:00",
                    "updated_at": "2022-11-22T10:10:31.000+07:00",
                    "name": "Singkawang Grand Mall"
                },
                {
                    "id": 183,
                    "voucher_id": 25,
                    "branch_id": 7,
                    "created_at": "2022-11-22T10:10:31.000+07:00",
                    "updated_at": "2022-11-22T10:10:31.000+07:00",
                    "name": "Summarecon"
                }
            ]
        },
        {
            "id": 26,
            "title": "Voucher F&B 20.000",
            "code": "UFB2c5B2w",
            "description": "S&K. minimum pembelanjaan 50ribu dan wajib purchase durasi waktu minimal 30 menit",
            "value": 90000,
            "max_value": 90000,
            "value_type": "price",
            "voucher_type": "discount",
            "start_date": "2022-11-22T03:12:02.000+07:00",
            "expired_date": "2022-11-29T00:00:00.000+07:00",
            "quantity": 1,
            "created_at": "2022-11-22T10:12:10.000+07:00",
            "updated_at": "2022-11-22T10:12:10.000+07:00",
            "is_enable": true,
            "actor": "promotion",
            "status": "pending",
            "branches": [
                {
                    "id": 184,
                    "voucher_id": 26,
                    "branch_id": 1,
                    "created_at": "2022-11-22T10:12:10.000+07:00",
                    "updated_at": "2022-11-22T10:12:10.000+07:00",
                    "name": "Summarecon Mall Serpong"
                },
                {
                    "id": 185,
                    "voucher_id": 26,
                    "branch_id": 2,
                    "created_at": "2022-11-22T10:12:10.000+07:00",
                    "updated_at": "2022-11-22T10:12:10.000+07:00",
                    "name": "Startspace Gading Serpong"
                },
                {
                    "id": 186,
                    "voucher_id": 26,
                    "branch_id": 3,
                    "created_at": "2022-11-22T10:12:10.000+07:00",
                    "updated_at": "2022-11-22T10:12:10.000+07:00",
                    "name": "Posbloc"
                },
                {
                    "id": 187,
                    "voucher_id": 26,
                    "branch_id": 5,
                    "created_at": "2022-11-22T10:12:10.000+07:00",
                    "updated_at": "2022-11-22T10:12:10.000+07:00",
                    "name": "Kantor Alsut"
                },
                {
                    "id": 188,
                    "voucher_id": 26,
                    "branch_id": 6,
                    "created_at": "2022-11-22T10:12:10.000+07:00",
                    "updated_at": "2022-11-22T10:12:10.000+07:00",
                    "name": "Singkawang Grand Mall"
                },
                {
                    "id": 189,
                    "voucher_id": 26,
                    "branch_id": 7,
                    "created_at": "2022-11-22T10:12:10.000+07:00",
                    "updated_at": "2022-11-22T10:12:10.000+07:00",
                    "name": "Summarecon"
                }
            ]
        },
        {
            "id": 27,
            "title": "Voucher F&B 20.000",
            "code": "UFBz7l2pH",
            "description": "S&K. minimum pembelanjaan 50ribu dan wajib purchase durasi waktu minimal 30 menit",
            "value": 90000,
            "max_value": 90000,
            "value_type": "price",
            "voucher_type": "discount",
            "start_date": "2022-11-23T05:09:55.000+07:00",
            "expired_date": "2022-11-30T00:00:00.000+07:00",
            "quantity": 1,
            "created_at": "2022-11-23T12:10:03.000+07:00",
            "updated_at": "2022-11-23T12:10:03.000+07:00",
            "is_enable": true,
            "actor": "promotion",
            "status": "pending",
            "branches": [
                {
                    "id": 190,
                    "voucher_id": 27,
                    "branch_id": 1,
                    "created_at": "2022-11-23T12:10:03.000+07:00",
                    "updated_at": "2022-11-23T12:10:03.000+07:00",
                    "name": "Summarecon Mall Serpong"
                },
                {
                    "id": 191,
                    "voucher_id": 27,
                    "branch_id": 2,
                    "created_at": "2022-11-23T12:10:03.000+07:00",
                    "updated_at": "2022-11-23T12:10:03.000+07:00",
                    "name": "Startspace Gading Serpong"
                },
                {
                    "id": 192,
                    "voucher_id": 27,
                    "branch_id": 3,
                    "created_at": "2022-11-23T12:10:03.000+07:00",
                    "updated_at": "2022-11-23T12:10:03.000+07:00",
                    "name": "Posbloc"
                },
                {
                    "id": 193,
                    "voucher_id": 27,
                    "branch_id": 5,
                    "created_at": "2022-11-23T12:10:03.000+07:00",
                    "updated_at": "2022-11-23T12:10:03.000+07:00",
                    "name": "Kantor Alsut"
                },
                {
                    "id": 194,
                    "voucher_id": 27,
                    "branch_id": 6,
                    "created_at": "2022-11-23T12:10:03.000+07:00",
                    "updated_at": "2022-11-23T12:10:03.000+07:00",
                    "name": "Singkawang Grand Mall"
                },
                {
                    "id": 195,
                    "voucher_id": 27,
                    "branch_id": 7,
                    "created_at": "2022-11-23T12:10:03.000+07:00",
                    "updated_at": "2022-11-23T12:10:03.000+07:00",
                    "name": "Summarecon"
                }
            ]
        },
        {
            "id": 28,
            "title": "Voucher F&B 20.000",
            "code": "UFBflAFMs",
            "description": "S&K. minimum pembelanjaan 50ribu dan wajib purchase durasi waktu minimal 30 menit",
            "value": 90000,
            "max_value": 90000,
            "value_type": "price",
            "voucher_type": "discount",
            "start_date": "2022-11-23T05:27:10.000+07:00",
            "expired_date": "2022-11-30T00:00:00.000+07:00",
            "quantity": 1,
            "created_at": "2022-11-23T12:27:19.000+07:00",
            "updated_at": "2022-11-23T12:27:19.000+07:00",
            "is_enable": true,
            "actor": "promotion",
            "status": "pending",
            "branches": [
                {
                    "id": 196,
                    "voucher_id": 28,
                    "branch_id": 1,
                    "created_at": "2022-11-23T12:27:19.000+07:00",
                    "updated_at": "2022-11-23T12:27:19.000+07:00",
                    "name": "Summarecon Mall Serpong"
                },
                {
                    "id": 197,
                    "voucher_id": 28,
                    "branch_id": 2,
                    "created_at": "2022-11-23T12:27:19.000+07:00",
                    "updated_at": "2022-11-23T12:27:19.000+07:00",
                    "name": "Startspace Gading Serpong"
                },
                {
                    "id": 198,
                    "voucher_id": 28,
                    "branch_id": 3,
                    "created_at": "2022-11-23T12:27:19.000+07:00",
                    "updated_at": "2022-11-23T12:27:19.000+07:00",
                    "name": "Posbloc"
                },
                {
                    "id": 199,
                    "voucher_id": 28,
                    "branch_id": 5,
                    "created_at": "2022-11-23T12:27:19.000+07:00",
                    "updated_at": "2022-11-23T12:27:19.000+07:00",
                    "name": "Kantor Alsut"
                },
                {
                    "id": 200,
                    "voucher_id": 28,
                    "branch_id": 6,
                    "created_at": "2022-11-23T12:27:19.000+07:00",
                    "updated_at": "2022-11-23T12:27:19.000+07:00",
                    "name": "Singkawang Grand Mall"
                },
                {
                    "id": 201,
                    "voucher_id": 28,
                    "branch_id": 7,
                    "created_at": "2022-11-23T12:27:19.000+07:00",
                    "updated_at": "2022-11-23T12:27:19.000+07:00",
                    "name": "Summarecon"
                }
            ]
        },
        {
            "id": 29,
            "title": "Voucher F&B 20.000",
            "code": "UFBFsQoiS",
            "description": "S&K. minimum pembelanjaan 50ribu dan wajib purchase durasi waktu minimal 30 menit",
            "value": 90000,
            "max_value": 90000,
            "value_type": "price",
            "voucher_type": "discount",
            "start_date": "2022-11-23T07:21:19.000+07:00",
            "expired_date": "2022-11-30T00:00:00.000+07:00",
            "quantity": 1,
            "created_at": "2022-11-23T14:21:19.000+07:00",
            "updated_at": "2022-11-23T14:21:19.000+07:00",
            "is_enable": true,
            "actor": "promotion",
            "status": "pending",
            "branches": [
                {
                    "id": 202,
                    "voucher_id": 29,
                    "branch_id": 1,
                    "created_at": "2022-11-23T14:21:19.000+07:00",
                    "updated_at": "2022-11-23T14:21:19.000+07:00",
                    "name": "Summarecon Mall Serpong"
                },
                {
                    "id": 203,
                    "voucher_id": 29,
                    "branch_id": 2,
                    "created_at": "2022-11-23T14:21:19.000+07:00",
                    "updated_at": "2022-11-23T14:21:19.000+07:00",
                    "name": "Startspace Gading Serpong"
                },
                {
                    "id": 204,
                    "voucher_id": 29,
                    "branch_id": 3,
                    "created_at": "2022-11-23T14:21:19.000+07:00",
                    "updated_at": "2022-11-23T14:21:19.000+07:00",
                    "name": "Posbloc"
                },
                {
                    "id": 205,
                    "voucher_id": 29,
                    "branch_id": 5,
                    "created_at": "2022-11-23T14:21:19.000+07:00",
                    "updated_at": "2022-11-23T14:21:19.000+07:00",
                    "name": "Kantor Alsut"
                },
                {
                    "id": 206,
                    "voucher_id": 29,
                    "branch_id": 6,
                    "created_at": "2022-11-23T14:21:19.000+07:00",
                    "updated_at": "2022-11-23T14:21:19.000+07:00",
                    "name": "Singkawang Grand Mall"
                },
                {
                    "id": 207,
                    "voucher_id": 29,
                    "branch_id": 7,
                    "created_at": "2022-11-23T14:21:19.000+07:00",
                    "updated_at": "2022-11-23T14:21:19.000+07:00",
                    "name": "Summarecon"
                }
            ]
        },
        {
            "id": 30,
            "title": "Voucher F&B 20.000",
            "code": "UFB2vhfu2",
            "description": "S&K. minimum pembelanjaan 50ribu dan wajib purchase durasi waktu minimal 30 menit",
            "value": 90000,
            "max_value": 90000,
            "value_type": "price",
            "voucher_type": "discount",
            "start_date": "2022-11-23T08:46:14.000+07:00",
            "expired_date": "2022-11-30T00:00:00.000+07:00",
            "quantity": 1,
            "created_at": "2022-11-23T15:46:14.000+07:00",
            "updated_at": "2022-11-23T15:46:14.000+07:00",
            "is_enable": true,
            "actor": "promotion",
            "status": "pending",
            "branches": [
                {
                    "id": 208,
                    "voucher_id": 30,
                    "branch_id": 1,
                    "created_at": "2022-11-23T15:46:14.000+07:00",
                    "updated_at": "2022-11-23T15:46:14.000+07:00",
                    "name": "Summarecon Mall Serpong"
                },
                {
                    "id": 209,
                    "voucher_id": 30,
                    "branch_id": 2,
                    "created_at": "2022-11-23T15:46:14.000+07:00",
                    "updated_at": "2022-11-23T15:46:14.000+07:00",
                    "name": "Startspace Gading Serpong"
                },
                {
                    "id": 210,
                    "voucher_id": 30,
                    "branch_id": 3,
                    "created_at": "2022-11-23T15:46:14.000+07:00",
                    "updated_at": "2022-11-23T15:46:14.000+07:00",
                    "name": "Posbloc"
                },
                {
                    "id": 211,
                    "voucher_id": 30,
                    "branch_id": 5,
                    "created_at": "2022-11-23T15:46:14.000+07:00",
                    "updated_at": "2022-11-23T15:46:14.000+07:00",
                    "name": "Kantor Alsut"
                },
                {
                    "id": 212,
                    "voucher_id": 30,
                    "branch_id": 6,
                    "created_at": "2022-11-23T15:46:14.000+07:00",
                    "updated_at": "2022-11-23T15:46:14.000+07:00",
                    "name": "Singkawang Grand Mall"
                },
                {
                    "id": 213,
                    "voucher_id": 30,
                    "branch_id": 7,
                    "created_at": "2022-11-23T15:46:14.000+07:00",
                    "updated_at": "2022-11-23T15:46:14.000+07:00",
                    "name": "Summarecon"
                }
            ]
        },
        {
            "id": 31,
            "title": "Voucher F&B 20.000",
            "code": "UFBxxJsPn",
            "description": "S&K. minimum pembelanjaan 50ribu dan wajib purchase durasi waktu minimal 30 menit",
            "value": 90000,
            "max_value": 90000,
            "value_type": "price",
            "voucher_type": "discount",
            "start_date": "2022-11-24T07:39:39.000+07:00",
            "expired_date": "2022-12-01T00:00:00.000+07:00",
            "quantity": 1,
            "created_at": "2022-11-24T14:39:39.000+07:00",
            "updated_at": "2022-11-24T14:39:39.000+07:00",
            "is_enable": true,
            "actor": "promotion",
            "status": "pending",
            "branches": [
                {
                    "id": 214,
                    "voucher_id": 31,
                    "branch_id": 1,
                    "created_at": "2022-11-24T14:39:39.000+07:00",
                    "updated_at": "2022-11-24T14:39:39.000+07:00",
                    "name": "Summarecon Mall Serpong"
                },
                {
                    "id": 215,
                    "voucher_id": 31,
                    "branch_id": 2,
                    "created_at": "2022-11-24T14:39:39.000+07:00",
                    "updated_at": "2022-11-24T14:39:39.000+07:00",
                    "name": "Startspace Gading Serpong"
                },
                {
                    "id": 216,
                    "voucher_id": 31,
                    "branch_id": 3,
                    "created_at": "2022-11-24T14:39:39.000+07:00",
                    "updated_at": "2022-11-24T14:39:39.000+07:00",
                    "name": "Posbloc"
                },
                {
                    "id": 217,
                    "voucher_id": 31,
                    "branch_id": 5,
                    "created_at": "2022-11-24T14:39:39.000+07:00",
                    "updated_at": "2022-11-24T14:39:39.000+07:00",
                    "name": "Kantor Alsut"
                },
                {
                    "id": 218,
                    "voucher_id": 31,
                    "branch_id": 6,
                    "created_at": "2022-11-24T14:39:39.000+07:00",
                    "updated_at": "2022-11-24T14:39:39.000+07:00",
                    "name": "Singkawang Grand Mall"
                },
                {
                    "id": 219,
                    "voucher_id": 31,
                    "branch_id": 7,
                    "created_at": "2022-11-24T14:39:39.000+07:00",
                    "updated_at": "2022-11-24T14:39:39.000+07:00",
                    "name": "Summarecon"
                }
            ]
        },
        {
            "id": 32,
            "title": "Voucher F&B 20.000",
            "code": "UFBm0DQsX",
            "description": "S&K. minimum pembelanjaan 50ribu dan wajib purchase durasi waktu minimal 30 menit",
            "value": 90000,
            "max_value": 90000,
            "value_type": "price",
            "voucher_type": "discount",
            "start_date": "2022-11-25T11:30:38.000+07:00",
            "expired_date": "2022-12-02T00:00:00.000+07:00",
            "quantity": 1,
            "created_at": "2022-11-25T18:30:38.000+07:00",
            "updated_at": "2022-11-25T18:30:38.000+07:00",
            "is_enable": true,
            "actor": "promotion",
            "status": "pending",
            "branches": [
                {
                    "id": 220,
                    "voucher_id": 32,
                    "branch_id": 1,
                    "created_at": "2022-11-25T18:30:38.000+07:00",
                    "updated_at": "2022-11-25T18:30:38.000+07:00",
                    "name": "Summarecon Mall Serpong"
                },
                {
                    "id": 221,
                    "voucher_id": 32,
                    "branch_id": 2,
                    "created_at": "2022-11-25T18:30:38.000+07:00",
                    "updated_at": "2022-11-25T18:30:38.000+07:00",
                    "name": "Startspace Gading Serpong"
                },
                {
                    "id": 222,
                    "voucher_id": 32,
                    "branch_id": 3,
                    "created_at": "2022-11-25T18:30:38.000+07:00",
                    "updated_at": "2022-11-25T18:30:38.000+07:00",
                    "name": "Posbloc"
                },
                {
                    "id": 223,
                    "voucher_id": 32,
                    "branch_id": 5,
                    "created_at": "2022-11-25T18:30:38.000+07:00",
                    "updated_at": "2022-11-25T18:30:38.000+07:00",
                    "name": "Kantor Alsut"
                },
                {
                    "id": 224,
                    "voucher_id": 32,
                    "branch_id": 6,
                    "created_at": "2022-11-25T18:30:38.000+07:00",
                    "updated_at": "2022-11-25T18:30:38.000+07:00",
                    "name": "Singkawang Grand Mall"
                },
                {
                    "id": 225,
                    "voucher_id": 32,
                    "branch_id": 7,
                    "created_at": "2022-11-25T18:30:38.000+07:00",
                    "updated_at": "2022-11-25T18:30:38.000+07:00",
                    "name": "Summarecon"
                }
            ]
        }
    ]
}
````
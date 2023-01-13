## Redeem Voucher

### Endpoint
````
[POST] url/redeem/reedemvoucher/ 
````

### POST Method
Use this ``json`` file with the format below to redeem voucher.
````
{
    "userid" : 2,
    "idvoucher" : 2,
    "kodevoucher" : "(confidential data)",
    "point" : 10,
    "coin" : 10
}
````
### Result
````
{
    "message": "successfully",
    "status": true,
    "count": 1,
    "results": {
        "voucher": [
            {
                "id_voucher": 2,
                "nama_voucher": "Free SInging 60 minutes",
                "jenis": 0,
                "kode_voucher": "(confidential data)",
                "kode_voucher_merchand": "(confidential data)",
                "expired": "2022-06-14T00:00:00",
                "url": "https://(confidential data)/",
                "point": 40,
                "coin": 40,
                "ketentuan": "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed ut eleifend velit. Aliquam pharetra mi ac felis elementum, eget congue enim dapibus. Mauris semper velit vitae tincidunt pretium. Donec ultricies purus sed leo commodo placerat. Aenean vehicula tristique sem a sagittis. Fusce non lorem consectetur, porta nisl id, consectetur sem. Nullam ipsum dolor, finibus vel ornare et, aliquam quis justo. Mauris enim diam, fermentum in fringilla quis, suscipit sit amet libero. Maecenas facilisis metus vitae auctor aliquam. Vestibulum sed sapien sed sem fringilla feugiat at sit amet est.",
                "id_siap": (confidential data)
            }
        ],
        "user": [
            {
                "id": 2,
                "reward": 0,
                "point": 225,
                "coin": 80,
                "phone_number": "(confidential data)",
                "pin": "(confidential data)",
                "code": (confidential data),
                "status": 0,
                "count_referal": 0,
                "idgetplus": "0",
                "membergetplus": "0",
                "extradata": null
            }
        ],
        "value": 40
    }
}
````

### Error Condition
````
If redeem voucher 2 times with the same kodevoucher.
{
    "message": "unsuccessfully",
    "status": false,
    "count": 1,
    "results": "duplicate voucher"
}

If send wrong kodevoucher. 
{
    "message": "unsuccessfully",
    "status": false,
    "count": 1,
    "results": "code is wrong"
}
````
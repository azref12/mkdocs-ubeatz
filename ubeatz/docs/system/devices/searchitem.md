## Devices > Search Item

### Endpoint
````
[GET] url/devices/booth-devices-details/?namadevices=(confidential data)
````

### GET Method
For *GET* method, use *namadevices* as ``params``.

### Result GET Method
````
{
    "message": "successfully",
    "status": true,
    "count": 1,
    "results": {
        "devices": [
            {
                "iddevices": 3,
                "namadevices": "(confidential data)",
                "nama": "(confidential data)",
                "status": 1,
                "players": 1,
                "codeconnect": "(confidential data)",
                "jam": null,
                "userid": null,
                "durasi": 4,
                "addtime": 2,
                "codeoutlet": "UBT",
                "idtransaksi": null,
                "ipaddress": "(confidential data)",
                "user": null
            }
        ]
    }
}
````
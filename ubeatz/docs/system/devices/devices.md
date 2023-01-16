## Devices

### Endpoint
````
[POST] url/devices/booth-devices/
````
````
[GET] url/devices/booth-devices/ 
````
````
[PUT] url/devices/booth-devices/?namadevices=(confidential data)
````

### POST Method
Use this ``json`` file with the format below to insert devices.
````
{
    "namadevices" : "(confidential data)",
    "status" : 1,
    "players" : 1,
    "durasi" : 4,
    "addtime" : 2,
    "codeconnect" : "(confidential data)",
    "codeoutlet" : "UBT",
    "namabooth" : "(confidential data)",
    "ipadd" : "(confidential data)"
}
````

### PUT Method
For *PUT* method, use *namadevices* as ``params``.

![params_putmethod](paramputdevices.png)

and also, add this ``json`` file with the format below to update devices.
````
{
    "codeconnect" : (confidential data),
    "code" : "UBT",
    "namabooth" : "(confidential data)"
}
```` 

### Result POST Method
````
{
    "message": "successfully",
    "status": true,
    "count": 1,
    "results": {
        "devices": [
            {
                "iddevices": (confidential data),
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
        ],
        "tools": [
            {
                "id": (confidential data),
                "runtext": [
                    {
                        "text": "Selamat Datang Di Karaoke"
                    },
                    {
                        "text": "Free 1 Jam Gratis 1 Jam"
                    },
                    {
                        "text": "Discount 10% Khusus Member"
                    }
                ],
                "promo": [
                    {
                        "path": "http://(confidential data)/imgpromo/1.png"
                    },
                    {
                        "path": "http://(confidential data)/imgpromo/2.png"
                    },
                    {
                        "path": "http://(confidential data)/imgpromo/3.png"
                    },
                    {
                        "path": "http://(confidential data)/imgpromo/4.png"
                    }
                ],
                "opening": [
                    {
                        "path": "http://(confidential data)/promo.mp4"
                    }
                ],
                "setting": [
                    {
                        "urlserver_lagu": "http://(confidential data)/data/"
                    }
                ],
                "code": "UBT",
                "keterangan": "Ubeatz"
            }
        ]
    }
}
````

### Result GET Method
````
{
    "message": "successfully",
    "status": true,
    "count": 1,
    "results": {
        "devices": [
            {
                "iddevices": (confidential data),
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

### Result PUT Method
````
{
    "message": "successfully",
    "status": true,
    "count": 1,
    "results": {
        "devices": [
            {
                "iddevices": (confidential data),
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
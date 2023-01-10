## Tools > Search by Code

Endpoint
````
[GET] url/tools/devices-details/?code=ALS 
````

## GET Method
For *GET* method, use *code* as ``params``.

## Result GET Method
````
{
    "message": "successfully",
    "status": true,
    "count": 1,
    "results": {
        "devices": [
            {
                "id": 2,
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
                        "path": "http://8.215.47.1/imgpromo/1.png"
                    },
                    {
                        "path": "http://8.215.47.1/imgpromo/2.png"
                    },
                    {
                        "path": "http://8.215.47.1/imgpromo/3.png"
                    }
                ],
                "opening": [
                    {
                        "path": "http://8.215.47.1/promo.mp4"
                    }
                ],
                "setting": [
                    {
                        "urlserver_lagu": "http://8.215.47.1/booth/lagu/"
                    }
                ],
                "code": "ALS",
                "keterangan": "Ubeatz"
            }
        ]
    }
}
````
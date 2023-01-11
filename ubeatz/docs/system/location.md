## Location

### Endpoint
````
[POST] url/location/location/
````
````
[GET] url/location/location/?open=1 
````

### POST Method
Use this ``json`` file with the format below to insert location.
````
{
    "place": "Pos Bloc Jakarta Phase 2 Lt. 1",
    "address": "Pos No.2, Ps.Baru, Kecamatan Sawah Besar, Kota Jakarta Pusat, Daerah Khusus Ibukota Jakarta 10710",
    "link": "https://goo.gl/maps/LsND2V2XcYjCM1Ht5",
    "open": 1
}
````

### GET Method
Use *open* as ``params`` to get location.

### Result POST Method
````
{
    "message": "successfully",
    "results": {
        "master": [
            {
                "id": 2,
                "place": "Pos Bloc Jakarta Phase 2 Lt. 1",
                "address": "Pos No.2, Ps.Baru, Kecamatan Sawah Besar, Kota Jakarta Pusat, Daerah Khusus Ibukota Jakarta 10710",
                "link": "https://goo.gl/maps/LsND2V2XcYjCM1Ht5",
                "open": 1
            }
        ]
    }
}
````

### Result GET Method
````
{
    "message": "successfully",
    "results": [
        {
            "id": 2,
            "place": "Pos Bloc Jakarta Lt.2 East Garden",
            "address": "Pos No.2, Ps. Baru, Kecamatan Sawah Besar, Kota Jakarta Pusat, Daerah Khusus Ibukota Jakarta 10710",
            "link": "https://goo.gl/maps/LsND2V2XcYjCM1Ht5",
            "open": 1
        }
    ],
    "success": true
}
````
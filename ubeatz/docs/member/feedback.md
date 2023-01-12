## Feedback 
### Endpoint
````
[POST] url/feedback/feedback/ 
````
````
[GET] url/feedback/feedback/ 
````

### POST Method
Use this ``json`` file with the format below to insert feedback.
````
{
    "userid": 2,
    "duration": "4",
    "location": "SMS",
    "Sound": "exc",
    "Song": "exc",
    "FandB": "exc",
    "staff": "exc",
    "area_clean": "exc",
    "sugest_song": "padi - semua tak sama"
}
````
### Result POST Method
````
{
    "message": "successfully",
    "results": {
        "master": [
            {
                "id": 2,
                "create_at": "2022-12-29T06:05:24.186663",
                "userid": 2,
                "duration": "4",
                "location": "SMS",
                "Sound": "exc",
                "Song": "exc",
                "FandB": "exc",
                "staff": "exc",
                "area_clean": "exc",
                "sugest_song": "padi - semua tak sama"
            }
        ]
    },
    "success": true
}
````

### Result GET Method
````
{
    "message": "successfully",
    "results": [
        {
            "id": 1,
            "create_at": "2022-12-29T06:05:03.851498",
            "userid": 163,
            "duration": "30",
            "location": "SMS",
            "Sound": "exc",
            "Song": "exc",
            "FandB": "exc",
            "staff": "exc",
            "area_clean": "exc",
            "sugest_song": "padi - semua tak sama"
        },
        {
            "id": 2,
            "create_at": "2022-12-29T06:05:24.186663",
            "userid": 2,
            "duration": "4",
            "location": "SMS",
            "Sound": "exc",
            "Song": "exc",
            "FandB": "exc",
            "staff": "exc",
            "area_clean": "exc",
            "sugest_song": "padi - semua tak sama"
        }
    ]
}
````
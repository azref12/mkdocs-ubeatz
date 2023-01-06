## Feedback 
Endpoint
````
[POST] url/feedback/feedback/ 
````

## POST Method
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
## Result 
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
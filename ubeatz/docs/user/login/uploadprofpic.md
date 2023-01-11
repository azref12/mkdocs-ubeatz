## Upload Profile Picture

### Endpoint
````
[POST] url/user/upload/ 
````
````
[GET] url/user/upload/ 
````

### POST Method
for *POST* method, add this in ``params``.

![upload_profpic](paramuploadprofpic.png)

### Result POST Method
````
{
    "Status": true,
    "message": "Image upload successfully",
    "results": {
        "id_up": 1,
        "id": 2,
        "profile": "http://192.168.18.9:8000/user/upload/media/profile/user.png"
    }
}
````
### Result GET Method
````
{
    "status": true,
    "message": "Successfully",
    "results": [
        {
            "id_up": 1,
            "id": 2,
            "profile": "media/profile/user.png"
        }
    ]
}
````
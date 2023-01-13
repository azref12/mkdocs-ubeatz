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
        "profile": "http://(confidential data)/user/upload/media/profile/user.png"
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
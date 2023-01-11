## Voucher

### Endpoint
````
[POST] url/voucher/voucher_list/
````
````
[GET] url/voucher/voucher_list/
````

### POST Method
Use this ``json`` file with the format below to insert voucher.
````
{
    "nama_voucher": "Free SInging 60 minutes",
    "jenis": "0",
    "kode_voucher_merchand": "abc12defz",
    "expired": "2022-06-14 00:00:00.000000",
    "url": "https://source.unsplash.com/user/c_v_r/",
    "point": "40",
    "coin": "40",
    "ketentuan": "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed ut eleifend velit. Aliquam pharetra mi ac felis elementum, eget congue enim dapibus. Mauris semper velit vitae tincidunt pretium. Donec ultricies purus sed leo commodo placerat. Aenean vehicula tristique sem a sagittis. Fusce non lorem consectetur, porta nisl id, consectetur sem. Nullam ipsum dolor, finibus vel ornare et, aliquam quis justo. Mauris enim diam, fermentum in fringilla quis, suscipit sit amet libero. Maecenas facilisis metus vitae auctor aliquam. Vestibulum sed sapien sed sem fringilla feugiat at sit amet est.",
    "id_siap": 29,
    "kode_voucher": "ASDFG12"
}
````

### Result POST Method
````
{
    "message": "successfully",
    "results": {
        "master": [
            {
                "id_voucher": 2,
                "nama_voucher": "Free SInging 60 minutes",
                "jenis": 0,
                "kode_voucher": "ASDFG12",
                "kode_voucher_merchand": "abc12defz",
                "expired": "2022-06-14T00:00:00",
                "url": "https://source.unsplash.com/user/c_v_r/",
                "point": 40,
                "coin": 40,
                "ketentuan": "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed ut eleifend velit. Aliquam pharetra mi ac felis elementum, eget congue enim dapibus. Mauris semper velit vitae tincidunt pretium. Donec ultricies purus sed leo commodo placerat. Aenean vehicula tristique sem a sagittis. Fusce non lorem consectetur, porta nisl id, consectetur sem. Nullam ipsum dolor, finibus vel ornare et, aliquam quis justo. Mauris enim diam, fermentum in fringilla quis, suscipit sit amet libero. Maecenas facilisis metus vitae auctor aliquam. Vestibulum sed sapien sed sem fringilla feugiat at sit amet est.",
                "id_siap": 29
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
            "id_voucher": 2,
            "nama_voucher": "Free SInging 60 minutes",
            "jenis": 0,
            "kode_voucher": "ASDFG12",
            "kode_voucher_merchand": "abc12defz",
            "expired": "2022-06-14T00:00:00",
            "url": "https://source.unsplash.com/user/c_v_r/",
            "point": 40,
            "coin": 40,
            "ketentuan": "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed ut eleifend velit. Aliquam pharetra mi ac felis elementum, eget congue enim dapibus. Mauris semper velit vitae tincidunt pretium. Donec ultricies purus sed leo commodo placerat. Aenean vehicula tristique sem a sagittis. Fusce non lorem consectetur, porta nisl id, consectetur sem. Nullam ipsum dolor, finibus vel ornare et, aliquam quis justo. Mauris enim diam, fermentum in fringilla quis, suscipit sit amet libero. Maecenas facilisis metus vitae auctor aliquam. Vestibulum sed sapien sed sem fringilla feugiat at sit amet est.",
            "id_siap": 29
        }
    ]
}
````
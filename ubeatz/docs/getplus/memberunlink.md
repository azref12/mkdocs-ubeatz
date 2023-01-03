## Member Unlink

Endpoint
````
[POST] {{partner_service_url}}/partner/v1/201904/members/unlink
````
````
[GET] {{base_url}}/mobile/v1/202001/utils/auth/partner-signature?PartnerID=f6348010-c54c-43d5-9f5e-be4c2562248d&EncryptKey=55HCmiPaEkEEy20LWP8V9nGbvpkl6EY8USqDkaRRlrk=&PartnerCustomerAccountID=fcea30ca-0f2a-449a-8ee7-71fa0d1b45bc&GetPlusID=6094450002009045855
````
to access unlink member, use the token obtained earlier at login as ``basic authentication``, on postman select ``authorization`` next to ``params``, then select ``Bearer Token``, then copy and paste token.

![bearertoken_memberunlink](img/token-memberunlink.png)

and also, select ``test`` and add this code.

![testmemberunlink](img/testmemberunlink.png)

after that, use this ``json`` file with the format below to post unlink member.
````
{
    "PartnerCustomerAccountID": "fcea30ca-0f2a-449a-8ee7-71fa0d1b45bc",
    "PartnerID": "f6348010-c54c-43d5-9f5e-be4c2562248d",
    "GetPlusID": "6094450002009045855",
    "Signature": "atAR2HIkfVCB+pU+T0QVewHMATCpdF+WgApEWJF/PH8=",
    "Timestamp": "1662111091"
}
````
for ``GET`` method, add this in ``params``.

![getmemberunlink](img/getmemberunlink.png)

## Result
````
{
    "ErrorCode": 0,
    "ErrorDescription": "",
    "Data": {
        "Timestamp": 1664343761,
        "Signature": "gPEHkwifUdCyiYTIfsL0cj7Lx7dSeBCBd1SbQyVLhe4=",
        "PartnerID": "f6348010-c54c-43d5-9f5e-be4c2562248d",
        "GetPlusID": "6094450002009045855"
    }
}
````
## Error Condition
Endpoint
````
[POST] {{partner_service_url}}/partner/v1/201904/members/unlink?access_token
````
## Error Result
if send link twice.
````
{
    "ErrorCode": -1,
    "ErrorDescription": "Account is already Linked"
}
````
if input invalid id
````
{
    "ErrorCode": -14,
    "ErrorDescription": "You are not authorize"
}
````
if input invalid partner id / id
````
{
    "ErrorCode": -4,
    "ErrorDescription": "Partner not found"
}
````
## Success Result
if unlink member success
````
{
    "ErrorCode": 0,
    "ErrorDescription": ""
}
````
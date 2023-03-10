## Member Unlink

### Endpoint
````
[POST] {{partner_service_url}}/partner/v1/201904/members/unlink
````
````
[GET] {{base_url}}/mobile/v1/202001/utils/auth/partner-signature?PartnerID=(confidential data)&EncryptKey=55HCmiPaEkEEy20LWP8V9nGbvpkl6EY8USqDkaRRlrk=&PartnerCustomerAccountID=(confidential data)&GetPlusID=(confidential data)
````
to access unlink member, use the token obtained from the previous ``partner token`` response as ``basic authentication``, on postman select ``authorization`` next to ``params``, then select ``Bearer Token``, then paste token.

![bearertoken_memberunlink](img/token-memberunlink.png)

### Test
and also, select ``test`` and add this code.

![testmemberunlink](img/testmemberunlink.png)

````
var jsonData = JSON.parse(responseBody);
if (jsonData.Data.Timestamp) {
    postman.setEnvironmentVariable("timestamp", jsonData.Data.Timestamp);
}
if (jsonData.Data.Signature) {
    postman.setEnvironmentVariable("signature", jsonData.Data.Signature);
}
if (jsonData.Data.PartnerID) {
    postman.setEnvironmentVariable("partner_id", jsonData.Data.PartnerID);
}
if (jsonData.Data.PartnerCustomerAccountID) {
    postman.setEnvironmentVariable("partner_customer_id", jsonData.Data.PartnerCustomerAccountID);
}
if (jsonData.Data.OTP) {
    postman.setEnvironmentVariable("otp_result", jsonData.Data.OTP);
}
if (jsonData.Data.GetPlusID) {
    postman.setEnvironmentVariable("getplus_id", jsonData.Data.GetPlusID);
}
````

### POST Method
Use this ``json`` file with the format below to insert unlink member.
````
{
    "PartnerCustomerAccountID": "(confidential data)",
    "PartnerID": "(confidential data)",
    "GetPlusID": "(confidential data)",
    "Signature": "atAR2HIkfVCB+pU+T0QVewHMATCpdF+WgApEWJF/PH8=",
    "Timestamp": "1662111091"
}
````
for `PartnerCustomerAccountID`,`PartnerID` and `GetplusID` is confidential data. So, use the previously obtained `PartnerCustomerAccountID`,`PartnerID` and `GetplusID`.

### GET Method
For *GET* method, add this in ``params``.

![getmemberunlink](img/getmemberunlink.png)

for `PartnerID`, `PartnerCustomerAccountID` and `GetplusID` is confidential data. So, use the previously obtained `PartnerID`, `PartnerCustomerAccountID` and `GetplusID`.

### Result POST Method
````
{
    "ErrorCode": 0,
    "ErrorDescription": "",
    "Data": {
        "Timestamp": 1664343761,
        "Signature": "gPEHkwifUdCyiYTIfsL0cj7Lx7dSeBCBd1SbQyVLhe4=",
        "PartnerID": "(confidential data)",
        "GetPlusID": "(confidential data)"
    }
}
````
### Result GET Method
If unlink member success
````
{
    "ErrorCode": 0,
    "ErrorDescription": ""
}
````
### Error Condition
If send link 2 times.
````
{
    "ErrorCode": -1,
    "ErrorDescription": "Account is already Linked"
}
````
If input invalid id.
````
{
    "ErrorCode": -14,
    "ErrorDescription": "You are not authorize"
}
````
If input invalid partner id / id.
````
{
    "ErrorCode": -4,
    "ErrorDescription": "Partner not found"
}
````
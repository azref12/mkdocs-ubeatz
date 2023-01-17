## Verify OTP

### Endpoint
````
[POST] {{partner_service_url}}/security/v1/201904/oauth/verify 
````
````
[GET] {{base_url}}/mobile/v1/202001/utils/auth/partner-signature?PartnerID=(confidential data)&EncryptKey=55HCmiPaEkEEy20LWP8V9nGbvpkl6EY8USqDkaRRlrk=&GetPlusID=(confidential data)
````
to verify OTP, use the token obtained from the previous ``partner token`` response as ``basic authentication``, on postman select ``authorization`` next to ``params``, then select ``Bearer Token``, then paste token.

![verifyotp_getplus](img/verifyotp.png)

### Test
and also, select ``test`` and  add this code.

![verify_test_getplus](img/testverifyotp.png)

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
````

### POST Method
Use this ``json`` file with the format below to verify OTP.
````
{
    "PartnerCustomerAccountID": "(confidential data)",
    "PartnerID": "(confidential data)",
    "GetPlusID": "(confidential data)",
    "Signature": "EROGkFQkA0kswYIsIZstEbirg8MxTStoY0ZwOvBpY4I=",
    "Timestamp": "1662101936",
	"OTP": "817270"
}
````
for `PartnerCustomerAccountID`,`PartnerID` and `GetplusID` is confidential data. So, use the previously obtained `PartnerCustomerAccountID`,`PartnerID` and `GetplusID`.

### GET Method
For *GET*  method, add this in ``params``.

![verify_getplus](img/getverifyotp.png)

for `PartnerID` and `GetplusID` is confidential data. So, use the previously obtained `PartnerID` and `GetplusID`.

### Result POST Method 
````
{
    "Data": {
        "MemberApplicationID": "(confidential data)",
        "JoinCode": 1,
        "MembershipNumber": "(confidential data)"
    },
    "ErrorCode": 0,
    "ErrorDescription": null
}
````
### Result GET Method 
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
### Error Condition
If the otp expired.
````
{
    "ErrorCode": -16,
    "ErrorDescription": "OTP code expired"
}
````
If the otp invalid.
````
{
    "ErrorCode": -16,
    "ErrorDescription": "OTP code expired"
}
````
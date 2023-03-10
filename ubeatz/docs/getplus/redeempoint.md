## Point Redeem

### Endpoint
````
[POST] https://partners-dev.gpiapis.com/partner/v1/201904/members/pointredeem
````
````
[GET] {{base_url}}/mobile/v1/202001/utils/auth/partner-signature?PartnerID=(confidential data)&EncryptKey=55HCmiPaEkEEy20LWP8V9nGbvpkl6EY8USqDkaRRlrk=&PartnerCustomerAccountID=(confidential data)&GetPlusID=(confidential data)&TransactionValue=1200
````
to access point redeem, use variables ``{{partner_access_token}}`` or you can use the token obtained from the previous ``partner token`` response as ``basic authentication``, on postman select ``authorization`` next to ``params``, then select ``Bearer Token``, then you choose one of the options above to be used as a token.

![redeem_point](img/tokenredeempoint.png)

### Test
and also, select ``test`` and add this code.

![testredeempoint](img/testredeempoint.png)

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
if (jsonData.Data.TransactionValue) {
    postman.setEnvironmentVariable("trans_value", jsonData.Data.TransactionValue);
}
````

### POST Method
Use this ``json`` file with the format below to insert point redeem.
````
{
    "PartnerID": "(confidential data)",
    "GetPlusID": "(confidential data)",
    "Signature": "5FrtmjEyJu4ofVIEQUZ/XBsymJxzzLE5CYtpCZH2s4Q=",
    "Timestamp": "1661859537",
    "TransactionValue": 1200,
    "TransactionID": "SO/(confidential data)/(confidential data)/(confidential data)",
    "TerminalID": "(confidential data)"
}
````
for `PartnerID`,`GetplusID`,`TransactionID` and `TerminalID` is confidential data. So, use the previously obtained `PartnerID`,`GetplusID`,`TransactionID` and `TerminalID`.

### GET Method
For *GET* method, add this in ``params``.

![getredeempoint](img/getredeempoint.png)

for `PartnerID`,`PartnerCustomerAccountID` and `GetplusID` is confidential data. So, use the previously obtained `PartnerID`,`PartnerCustomerAccountID` and `GetplusID`.

### Result
````
{
    "ErrorCode": 0,
    "ErrorDescription": "",
    "Data": {
        "LoyaltyPointsBalance": 766300,
        "TransactionID": "SO/(confidential data)/(confidential data)/(confidential data)",
        "TransactionSet_RSN": "(confidential data)"
    }
}
````
### Error Condition
If send same TransactionID 2 times.
````
{
    "ErrorCode": "20215",
    "ErrorDescription": "Duplicate Transaction ID"
}
````
If send invalid/empty/expired token.
````
{
    "ErrorCode": -12,
    "ErrorDescription": "You are not authorize"
}
````
If send invalid signature.
````
{
    "ErrorCode": -14,
    "ErrorDescription": "You are not authorize"
}
````
If send invalid/empty/expired token and sent invalid signature.
````
{
    "ErrorCode": -12,
    "ErrorDescription": "You are not authorize"
}
````
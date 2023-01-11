## Earn Point / Sale Transaction

### Endpoint
````
[POST] {{partner_service_url}}/partner/v1/201904/members/saletransaction
````
````
[GET] {{base_url}}/mobile/v1/202001/utils/auth/partner-signature?PartnerID=f6348010-c54c-43d5-9f5e-be4c2562248d&EncryptKey=55HCmiPaEkEEy20LWP8V9nGbvpkl6EY8USqDkaRRlrk=&PartnerCustomerAccountID=fcea30ca-0f2a-449a-8ee7-71fa0d1b45bc&GetPlusID=6094450002009045855&TransactionValue=50000
````
to access earn point / sale transaction, use variables ``{{partner_access_token}}`` or you can use the token obtained from the previous ``partner token`` response as ``basic authentication``, on postman select ``authorization`` next to ``params``, then select ``Bearer Token``, then you choose one of the options above to be used as a token.

![earn_point](img/tokenearnpoint.png)

### Test
and also, select ``test`` and add this code.

![testmemberunlink](img/testearnpoint.png)

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
Use this ``json`` file with the format below to insert earn point.
````
{
    "PartnerID": "f6348010-c54c-43d5-9f5e-be4c2562248d",
    "GetPlusID": "6094450002009045855",
    "Signature": "NgGMogyQeOxXgjW9E2giHFSivs13PphLVhB9m7CcUG8=",
    "Timestamp": "1661926366",
    "TransactionValue": 100000,
    "TransactionID": "GETPLUS/0221/002",
    "TerminalID": "10001"
}
````
### GET Method
For *GET* method, add this in ``params``.

![getmemberunlink](img/getearnpoint.png)

### Result
````
{
    "ErrorCode": 0,
    "ErrorDescription": "",
    "Data": {
        "LoyaltyPointsBalance": 767500,
        "TransactionID": "GETPLUS/0221/061",
        "TransactionSet_RSN": "b49d3c5f-1002-45e1-ac71-869fe4f6c977"
    }
}
````
### Error Condition
if send same TransactionID 2 times.
````
{
    "ErrorCode": "20215",
    "ErrorDescription": "Duplicate Transaction ID"
}
````
if send invalid/empty/expired token.
````
{
    "ErrorCode": -12,
    "ErrorDescription": "You are not authorize"
}
````
if send invalid signature.
````
{
    "ErrorCode": -14,
    "ErrorDescription": "You are not authorize"
}
````
if send invalid/empty/expired token and sent invalid signature.
````
{
    "ErrorCode": -12,
    "ErrorDescription": "You are not authorize"
}
````
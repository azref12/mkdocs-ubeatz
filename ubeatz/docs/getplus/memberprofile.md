## Member Profile

### Endpoint
````
[GET] {{partner_service_url}}/partner/v1/201904/members/(confidential data)
````
to get member profile, use the token obtained from the previous ``partner token`` response as ``basic authentication``, on postman select ``authorization`` next to ``params``, then select ``Bearer Token``, then paste token.

![tokenmemberprofile](img/tokenmemberprofile.png)

### Result
````
{
    "Data": {
        "AvailableBalance": 767200,
        "GivenName": "Gpi",
        "FamilyName": "Ubeatz",
        "EmailAddress": "(confidential data)",
        "PhoneNumber": "(confidential data)",
        "Program": "GPS",
        "MembershipNumber": "(confidential data)"
    },
    "ErrorCode": 0,
    "ErrorDescription": null
}
````
### Error Condition

If member non existing profile
````
{
    "ErrorCode": 30201,
    "ErrorDescription": "Member not found"
}
````
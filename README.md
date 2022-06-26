# Smitch-API
A **postman collection** and **openapi spec.** to control smitch smart devices including lights and switches.

Offical documentation for the Smitch Smart app control: [https://docs.developer.mysmitch.com](https://docs.developer.mysmitch.com). <br>
Offical "Get started" guide: [Get-Started](https://docs.developer.mysmitch.com/developer-portal/get-started).

## How to use the postman collection
### Prerequisites
Please familiarise yourself with the basic prerequisite at: [Prerequisites](https://docs.developer.mysmitch.com/#0.-prerequisites)
- Register a developer account at: [Developer-Portal](https://developer.mysmitch.com) by selecting Sign Up (Sign In if you already created an account)
- Add an App in your developer account and create a "TEST" API KEY. More details: [api-keys](https://docs.developer.mysmitch.com/app/api-keys). Save this api-key somewhere safe.
- Link a "tester" to your application. More details: [user-tester](https://docs.developer.mysmitch.com/users/user-tester), make sure the tester's account used here is the same as the one you use to sign in the Smitch mobile app.

### Using the collection.

1. Load the collection located at [collection](./Smitch&#32;Postman&#32;API&#32;collection.postman_collection.json) in your local/web instance of Postman.
2. Open the "Smitch Postman API collection", select the variables tab and set the "api_key" variable's value to your api_key obtained from.
3. Select the "Everything_is_valid" request and send it. If everything was done correctly, this should return a  "status": "success". If not, please validate your steps again.
4. Select the "list_of_users" request and send it. Obtain the user_id variable of the desired user (make sure the said account is added as tester as per above), add this key's value to your collection's variable "user_id" variable's value.
5. To control a device, you first need to identify it's "device_id" and add it in collection's variables. To obtain a list of all devices added in user's account please use the "get_user_details" request.

## To Be Done
 - ~~Check feasibility of converting this to openapi.~~ **Result**: Doable.
 - ~~Convert this to OpenAPI version 3 spec.~~
 - Use openapi and swagger-ui to host this in the form of a github page.
 - Customise the openapi.yaml spec to better suite the needs of the version.
 - Do test runs
 - Add documentation for using openapi.yaml to create SDKs, and finally be at peace ❤️

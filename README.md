# Smitch-Postman-API
A postman collection to control switch smart devices.

Offical documentation for the Smitch Smart app control: [https://docs.developer.mysmitch.com](https://docs.developer.mysmitch.com)

## How to use
### Prerequisites
Please familiarise yourself with the basic prerequisite at: [Prerequisites](https://docs.developer.mysmitch.com/#0.-prerequisites)
- Register a developer account at: [Developer-Portal](https://developer.mysmitch.com) by selecting Sign Up (Sign In if you already created an account)
- Add an App in your developer account and create a "TEST" API KEY. More details: [api-keys](https://docs.developer.mysmitch.com/app/api-keys). Save this api-key somewhere safe.
- Link a "tester" to your application. More details: [user-tester](https://docs.developer.mysmitch.com/users/user-tester), make sure the tester's account used here is the same as the one you use to sign in the Smitch mobile app.

### Using the collection.

1. Load the collection in your Postman.
2. Open the "Smitch Postman API collection", select the variables tab and set the "api_key" variable's value to your api_key obtained from.
3. Select the "Everything_is_valid" request and send it. If everything was done correctly, this should return a  "status": "success". If not, please validate your steps again.
4. Select the "list_of_users" request and send it. Obtain the user_id variable of the desired user (make sure the said account is added as tester as per above), add this key's value to your collection's variable "user_id" variable's value.
5. To control a device, you first need to identify it's "device_id" and add it in collection's variables. To obtain a list of all devices added in user's account please use the "get_user_details" request.

# Postman Collection for ACC Submittals API

[![Postman](https://img.shields.io/badge/Postman-v8-orange.svg)](https://www.getpostman.com/)

[![Autodesk Construction Cloud API](https://img.shields.io/badge/Autodesk%20Construction%20Cloud%20API-v1-green.svg)](https://aps.autodesk.com/en/docs/acc/v1/overview/)

![Beginner](https://img.shields.io/badge/Level-Beginner-green.svg)
[![License](https://img.shields.io/:license-MIT-blue.svg)](http://opensource.org/licenses/MIT)

This folder contains a Postman Collection that includes all the current ACC Submittals API. The collection together with the environment help you easily test these endpoints.

![Collection](img/collection.png)
![Tutorial](img/tutorial.png)


## Instructions to run the Postman collection are as below

### Setup Postman environment and Authorization
- Import Postman environment & collection, please setup the following environment vialables, 
    - client_id:     APS App Id.
    - client_secret: APS App Secret.

![Env](img/env.png)

- Please add the Authorization for the collection, click **Edit Collection**, go to **Authorization** tab, make sure to use **OAuth 2.0** to get a 3 legged token, use it in the **Request Headers**.
    - Callback URL: https://www.postman.com/oauth2/callback
    - Auth URL: https://developer.api.autodesk.com/authentication/v2/authorize
    - Access Token URL: https://developer.api.autodesk.com/authentication/v2/token

![3leggedToken](img/3leggedToken.png)

### Use the endpoints under **Run Firstly-Get Project ID** to set `project_id_without_b`, then you can play with any Endpoint as you want.

## Tips & Tricks
- These endpoints are used to quickly test/verify the endpoints. You need to set up the environment variables before running the Postman request.

## License
This sample is licensed under the terms of the [MIT License](http://opensource.org/licenses/MIT). Please see the [LICENSE](../LICENSE) file for full details.

## Written by
Eason Kang [@yiskang](https://twitter.com/yiskang), [Developer Advocacy and Support](http://aps.autodesk.com)

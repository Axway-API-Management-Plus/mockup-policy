# Description
This Sample-Policy allows you to control Mockup-Routing for API-Manager using tags configured for your APIs.

The policy supports Global-API-Level- or API-Method-Level-Mocking. Method-Level-Mocking overrules API-Mock-Settings.

![Mocksetting](https://github.com/Axway-API-Management-Plus/mockup-policy/blob/master/images/Mock-Tag-for-API.png)

For the example above the following is logged at runtime:
```
No API-Method mock-settings configured
API-Global mock-settings: true|http://localhost:4010/v2
No Mocking defined on operation
Using mockURL: http://localhost:4010/v2; isMocked: true
```
So finally the API-Gateway connects to the configured mock-host: http://localhost:4010/v2

You may use Mockup-Servers, like Prism (http://stoplight.io/platform/prism/) from stoplight.io providing you options to run Mock-Servers based on your Swagger-Definitions. 

## API Management Version Compatibilty
This artefact was successfully tested for the following versions:
- V7.5.3


## Install

```
• Import the Policy: "Is Mockup?" into your API-Manager configuration group
• Make this policy part of your API-Manager routing policy (e.g. using a Policy-Shortcut)
• If you don't have any routing policy you find an example in: MainRoutingPolicy
• Configure this routing poliy in API-Manager for your APIs
```

## Usage

```
• To enable mocking for a API, add a tag name: "mock"
• The value must have the following format: "<status>|<mockup-host>"
• Example: "true|http://mockserver:8080/api/v2"
• You may override this setting on per method level
• This example will disable mock for a specific method: "false" (the host isn't needed)
• In case global mockups are disabled, you can turn it on per API method just by adding the mock-details
```

## Bug and Caveats

```
No known bugs or caveats
```

## Contributing

Please read [Contributing.md](https://github.com/Axway-API-Management/Common/blob/master/Contributing.md) for details on our code of conduct, and the process for submitting pull requests to us.


## Team

![alt text][Axwaylogo] Axway Team

[Axwaylogo]: https://github.com/Axway-API-Management/Common/blob/master/img/AxwayLogoSmall.png  "Axway logo"


## License
[Apache License 2.0](/LICENSE)

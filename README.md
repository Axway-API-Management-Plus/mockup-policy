# Description
This Sample-Policy allows you to control Mockup-Routing for API-Manager using tags configured for your APIs.

The policy supports Global-API-Level- or API-Method-Level-Mocking. Method-Level-Mocking overrules API-Mock-Settings.

## API Management Version Compatibilty
This artefact was successfully tested for the following versions:
- V7.5.3


## Install

```
• Import the Policy: "Is Mockup?" into you API-Manager configuration group
• Make this policy part of your API-Manager routing policy (a Policy-Shortcut)
• If you don't have any routing policy you find an example in: MainRoutingPolicy
• Configure your routing poliy in API-Manager
```

## Usage

```
• To enable mocking for a API, add a tag name: "mock"
• The value have the following format: <status>|<mockbakend>
• Example: true|http://mockserver:8080/api/v2
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

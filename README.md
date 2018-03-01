# Swagger-Mock-Validator example Project

This test project uses the Atlassian swagger-mock-validator via the "test" script in package.json to verify a swagger spec file against a pact mock file.

## How to Run

Run `npm install` to load the needed javascript libraries and then `npm run test` to
run the tests. After the tests have successfully run the created pact file will be
created in the folder `pacts`. 

Then, you can call `npm run publish-pacts` to publish the pact files to a [Pact Broker](https://github.com/pact-foundation/pact_broker).
You must set the following npm configs for the `publish-pacts` script to work:

```
npm config set angular-pact:brokerUrl <URL>
npm config set angular-pact:brokerUsername <USER>
npm config set angular-pact:brokerPassword <PASS>

``` 

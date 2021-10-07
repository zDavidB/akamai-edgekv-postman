# akamai-edgekv-postman
Akamai EdgeKV API PostMan collection


Based on the EdgeKV API found here - https://github.com/akamai/edgeworkers-examples/tree/master/edgekv/apis#edgekv-api

A PostMan API collection and skeleton environment.

Clone the repo to your local drive, then import the collection and environment into a PostMan Workspace,

## To test, 
- Define a MockServer in Postman and set the hostname of the MockServer (without the `https://`) in the `host` variable of the environment.

- Each request has an example response that can be called from the corresponding request, with the request setting some example values in the requests `pre-request script`

## To use
- Get your friendly Akamai Engineering Admin person to create an Akamai IAM user, or ideally a Service Account API.

- You should be provided with a set of EdgeRC tokens (two tokens, one secret, and one host)

- In the PostMan Environment is a corresponding four variables, fill in the CURRENT VALUE with the tokens, secret and host and save the environment.
  - **IMPORTANT NOTE** - DO NOT SAVE THE VALUE IN THE `INITAL VALUE` FIELDS, these may be visible if you go one to share the enviroment, and expose the tokens.

- In the Collection, set the Autorization tab so the type field is `Akamai EdgeGrid`
  - Set the Access Token field to be {{access_token}}
  - Set the Client Token field to be {{client_token}}
  - Set the Client Secret field to be {{client_secret}}
  - The host is set on each request; note make sure the host value in the Environment variable does not contain `https://`


Some tests are written for each request.


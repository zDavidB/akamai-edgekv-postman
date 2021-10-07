# akamai-edgekv-postman
Akamai EdgeKV API PostMan collection


Based on the EdgeKV API found here - https://github.com/akamai/edgeworkers-examples/tree/master/edgekv/apis#edgekv-api

A PostMan API collection and skeleton environment.

To use, import the collection and environment into a Workspace, then define a MockServer in Postman and set the hostname of the MockServer (without the `https://`) in the `host` variable of the environment.

Each request has an example response that can be called from the corresponding request, with the request setting some example values in the requests `pre-request script`

Some tests are written for each request.


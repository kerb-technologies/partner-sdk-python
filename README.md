# partner-sdk-python
Kerb Partner SDK for Python


```python
from kerb import partner

// set KERB_PARTNER_HOST in your environment
// get your token from your kerb dashboard app
token = <your-token>
partner.set_apikey(token);

options = {
    "body": []
}

// partner.send use partner.request while do http request
// since we use axios for http request, so return is axion response
// see this for more information https://github.com/axios/axios#response-schema

response = partner.send('ping', options)

// use custom request object
request = partner.make_request('ping', options)
request.headers = {
    'testign': 'ok',
    'not-used': null,
}

response = partner.send('ping', options)


```

# Installation

TODO

# Configuration

TODO




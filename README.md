# SwiftShipper

Ecommerce platform with admin planel based on MERN stack and integrated payment gateway using Razorpay.

## Installation

1. clone the repo to your local

```

git clone https://github.com/amartyyya/SwiftShipper

```

2. Install dependencies

```
cd client && npm install
cd ../server && npm install
```

3. Start server and UI

Move to client directory to start frontend

```
npm start
```

Move to server directory to start backend server

```
npm start
```

### Additional

while starting client sever if you get this issue

```
Error: digital envelope routines::unsupported

opensslErrorStack: [ 'error:03000086:digital envelope routines::initialization error' ],
library: 'digital envelope routines',
reason: 'unsupported',
code: 'ERR_OSSL_EVP_UNSUPPORTED'
```

Then change the script in package.json in client to

```
"scripts": {
    "start": "react-scripts --openssl-legacy-provider start",
    "build": "react-scripts --openssl-legacy-provider build",
}
```
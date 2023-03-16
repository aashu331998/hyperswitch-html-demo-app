# hyperswitch-html-demo-app

A simple app to demo html integration of Hyperswitch

## Running the sample

1. Build the server

```
npm install or yarn
```

2. Provide valid Api key in server.js and Publishable key in checkout.js. You can create your keys using the Hyperswitch dashboard. https://app.hyperswitch.io/

```
//in server.js
const hyper = require("@juspay-tech/hyperswitch-node")("api_key");
```

```
//in checkout.js
const hyper = Hyper("publishable_key");
```

> Note: If you have migrated from Stripe, ensure that you have enabled the 'Handle card information directly' option under the Settings > Integration section of your Stripe dashboard to allow hyperswitch to securely process your customers' card details.

3. Run the server

```
npm start
```

4. Go to [http://localhost:4242/checkout.html](http://localhost:4242/checkout.html)

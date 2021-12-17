---
description: >-
  The Livquik Payments plugin allows you to accept credit card, UPI, Netbanking
  and debit card payments via Livquik payment gateway.
---

# Javascript Integration

## Configuration

Initialize your object by passing your order id and public key:

> Get Order Id from Create order api from next step

```javascript
<script type="text/javascript" src="https://merchantapi.livquik.com/scripts/livquik.v1.js"></script>
<script type="text/javascript">
var order_id;
var options = {
    "order_id" : order_id, //Get order_id params value from Create Order from next step
    "public_key" : "pk_live_xxxxxxxxx"
}
var lpay = new Livquik(options);
```

You can get your Public and Secret key from the api [dashboard](https://merchantapp.livquik.com/dashboard).

## Create Order

Create order from Server side using below API and get the Order id. [Click here](https://docs.livquik.com/server-side-integrations/rest-api) to know how to create a order.

## Open the payment view

Use the below code to open the payment view for the customers to pay.

```javascript
lpay.open();
```

## Close the payment view

Use the below code to close the payment view.

```javascript
lpay.close();
```

## Response Handlers

For Success and Error handlers use the below handler function for payment response

```javascript
livquikHandler(response, function (e) {
    if(e.data.status == 'success'){
        console.log(e.data)
    }
    if(e.data.status == 'failure'){
        console.log(e.data)
    }
});
```

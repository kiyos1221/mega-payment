Mega payment API. It allows to make payment using the users id to 

 - Another meda user
 - To Merchant
 - To phone number

## Getting started

Install the library using either Yarn:

    yarn add @mega/payment
or npm:

    npm install @mega/payment

## Compatibility

This version of mega payment is compatible with

| @mega/payment version | mega version  |
|--|--|
| 1.0.0 | 1.0.0 |

## Usage

import library
```javascript
import MegaPayment from '@mega/payment'
```

make payment
```javascript
    MegaPay.makePayment({
          medaUUID: ${USER_MEDA_ID},
          merchantId: ${MERCHANT_ID},
          amount: `${AMOUNT}`,
          paymentAction: '${PAYMENT_ACTION}',
          paymentLabel: `${PAYMENT_LABEL}`,
          metaData: '${META_DATA}',
          additionalInfo: [
            'CONTENT',
            ${KEY},
            ${VALUE},
          ],
        },
        response => {
          //Payment successfull
        },
        error => {
          //Payment error
        },
      );
```

## API

 - **Methods**
      - `makePayment()`

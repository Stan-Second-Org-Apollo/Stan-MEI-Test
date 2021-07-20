# Checkout Step Encountered

### 

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Checkout Step Encountered",
    "checkoutMethod": "<checkoutMethod>",
    "eventDetails": {
        "checkoutStep": "<checkoutStep>"
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|checkoutMethod|string|The checkout method associated with checkout activity.||||||||
|checkoutStep|string|Describes a discrete step in the checkout flow. |Cart Review, Billing Info, Shipping Info, Order Review|||||||

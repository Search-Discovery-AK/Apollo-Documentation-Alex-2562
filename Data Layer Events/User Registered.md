# User Registered

### 

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "sign_up",
  "apollo_event": "User Registered",
    "user": {
        "country": "<country>",
        "loyalty": {
            "isLoyaltyRegistration": <isLoyaltyRegistration>
        },
        "profileAttributesList": "<profileAttributesList>",
        "system": "<system>"
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|country|string|The country associated with this user's profile.|USA, Canada|||||||
|isLoyaltyRegistration|integer|User regsitered for a new Loyalty account.||||||||
|profileAttributesList|string|A twice delimited string of key \/ value pairs.  Use \~ between key and value.  Use \| between pairs|homeStore\~234\|loyaltyTier\~gold\|memberSince\~2002|||||||
|system|string|Describes the system that the user is logged into.  \(rarely used\). |admin, shop, member|||||||





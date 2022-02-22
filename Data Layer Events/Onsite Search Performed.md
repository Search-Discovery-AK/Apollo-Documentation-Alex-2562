# Onsite Search Performed

### 

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "search",
  "apollo_event": "Onsite Search Performed",
    "onsiteSearch": {
        "keyword": {
            "multiSearchEntries": "<multiSearchEntries>"
        },
        "location": {
            "locationID": "<locationID>",
            "map": {
                "vendor": "<vendor>",
                "zoomLevel": "<zoomLevel>"
            }
        },
        "scheduling": {
            "daysBeforeStartDate": <daysBeforeStartDate>,
            "endDate": "<endDate>",
            "requestedDatesCount": <requestedDatesCount>
        }
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|daysBeforeStartDate|integer|Integer Number of days until the requested start date \(same day = 0\)|0, 1, 5, 6, 7, 10||||0|||
|endDate|string|End date requested. ISO 8601 form \(YYYY-MM-DD\). Jan 1, 2019 is 2019-01-01|2001-12-22, 2011-01-01|^([0-9]{4})-(1[0-2]|0[1-9])-(3[01]|0[1-9]|[12][0-9])$||||||
|locationID|string|The Location Id requested in search criteria.|155, 65588, 987764448|||||||
|multiSearchEntries|string|The user's fields and values entered for multi-search.|fieldName\~phrase, sku\~12345, product name\~oak\|sku\~12345\|color\~green|||||||
|requestedDatesCount|integer|Integer Number of days requested.|8, 1, 5, 6, 7, 10||||1|||
|vendor|string|The technology vendor of the map|Google, Bing, Mapquest, ESRI|||||||
|zoomLevel|string|Indicator of the zoom level in a map presentation. Values are typically integers, but can vary depending on the map service used. |1, 2, 3, 4, 5, 6|||||||





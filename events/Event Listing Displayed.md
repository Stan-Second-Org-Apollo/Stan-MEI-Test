# Event Listing Displayed

### This event is part of the page load sequence, including virtual page loads in the case of single page apps, and must be pushed between the `Page Load Started` and `Page Load Completed` events.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Event Listing Displayed",
    "listingDisplayed": {
        "displayCount": "<displayCount>",
        "listing": [
            {
                "event": {
                    "eventId": "<eventId>",
                    "eventName": "<eventName>",
                    "eventType": "<eventType>",
                    "status": "<status>"
                },
                "itemPosition": "<itemPosition>"
            }
        ],
        "resultsCount": "<resultsCount>"
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|displayCount|integer|The total number of items displayed out of all returned items. \(Integer\)|10, 20, 30, 40||||0|||
|eventId|string|Unique Identifier of an event. |155, 65588, 987764448|||||||
|eventName|string|The friendly name of the event.|Max your 401K, Structured JavaScript, Mid Day Yoga, Frosty 5K Fun Run, Whiskey Wednesday|||||||
|eventType|string|The type of the event|Webinar, Class, Conference, Race, Meet Up|||||||
|itemPosition|integer|Integer position of a property within a sorted result. The first returned is position 1. For map results, this value can be the rank by distance from POI.|1, 2, 3, 4, 5||||0|||
|resultsCount|integer|The total number of items returned that matched the search criteria. \(Integer\)|1, 21, 111, 166||||0|||
|status|string|The status of an event.|Cancelled, Sold Out, Postponed, Rescheduled|||||||

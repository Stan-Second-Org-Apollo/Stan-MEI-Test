# Page Load Started

### Page Load Started is part of the page load sequence, including virtual page loads in the case of single page apps, and must be the first event pushed in the page load event sequence.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Page Load Started",
    "page": {
        "breadcrumbs": "<breadcrumbs>",
        "dayOfWeek": "<dayOfWeek>",
        "detailedPageName": "<detailedPageName>",
        "internalBusinessOwner": "<internalBusinessOwner>",
        "pageType": "<pageType>",
        "siteExperience": "<siteExperience>",
        "subsection": "<subsection>"
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|breadcrumbs|string|A delimited list of hierarchical sections that describe the current page's location within the navigation of the site.|Home&gt;Women&gt;Tops&gt;Sweaters, Mens - Tops - Sweaters - Supmina, Wool, Rayon, Checkout &gt; Order Thank You|||||||
|dayOfWeek|string|The day of the week the activity occured.||||||||
|detailedPageName|string|Describes the page in more detail than the pageName attribute|product - XYZ123 - super cotton neck scarf, Mens - Tops - Sweaters - Supmina, Wool, Rayon, Order Confirmation - 098fghjkl|||||||
|internalBusinessOwner|string|Describes the internal team who manages this particular page of the website.|XX product management, marketing, vendor name|||||||
|pageType|string|Describes what purpose the page serves. Often aligns with the CMS template.|Home, Event Detail, Property Detail, Product Listing, Blog Post, Shopping Cart|||||||
|siteExperience|string|Describes the version of the site that is being shown|Responsive, Mobile, Desktop|||||||
|subsection|string|First sub-level of hierarchy under pageCategory or Site Section. |Shop &gt; Kids, Shop &gt; Mens, Shop &gt; Womens|||||||

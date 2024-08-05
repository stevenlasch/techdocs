### Code: Get Query String Value

```
// Get the value for a query string value pair
function getQueryStringValue(variable) {
    if (variable) {
        var queryStringValue = null;

        // Get the entire queryString
        var queryString = window.location.search;
        queryString = queryString.substring(1);

        // Split the string into value pairs
        var queryStringPairs = queryString.split("&");

        for (var i = 0, l = queryStringPairs.length; i < l; i++) {
            var queryStringPair = queryStringPairs[i].split("=");
            
            if (queryStringPair[0] === variable) {
                queryStringValue = queryStringPair[1];
                break;
            }
        }

        return queryStringValue;
    } else {
        console.log("Error: `variable` is not defined for `getQueryStringValue`");
    }
}
```

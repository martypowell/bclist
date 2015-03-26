# bclist
Goal of this library is to make it super simple to GET data from County Web Services.

## dependencies
[jQuery](https://jquery.com/)

##usage
```javascript
(function($, BcList) {
    var resultList = new BcList({
        containerClass: "results-list", //Selector of class you want to append your results
        source: "webServiceUrl",
        templatePath: "localPathToTemplate"
    });

    $(document).ready(function() {
        resultList.Show();
    });
})(jQuery, BcList);

```
# bclist
Goal of this library is to make it super simple to GET data from County Web Services.

## dependencies
* [jQuery](https://jquery.com/)
* [Handlebars](http://handlebarsjs.com/)

##usage
Include jQuery, Handlebars and the bc.list.js whereever you put your js code in your app.

```html
<script src="your/path/to/jquery/jquery.js"></script>
<script src="your/path/to/jquery/handlebars.js"></script>
<script src="your/path/to/jquery/bc.list.js"></script>

```

```javascript
(function($, BcList) {
    var resultList = new BcList({
        containerClass: "results-list", //Name of the class you want to append your results to, do not include the dot(.)
        source: "webServiceUrl",
        templatePath: "localPathToTemplate"
    });

    $(document).ready(function() {
        resultList.Show();
    });
})(jQuery, BcList);

```

##example usage
http://www.baltimorecountymd.gov/Agencies/health/petadoption/

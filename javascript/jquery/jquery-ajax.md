## JavaScript: JQuery: AJAX

### AJAX: [How to convert an Ajax call to a Promise](https://dev.to/gishan_abeysinghe/how-to-convert-an-ajax-call-to-a-promise-bd0)
```
function ajaxPromise(data, url, type) {
   return new Promise(function (resolve, reject) {
        $.ajax({
          type,
          url,
          data,
          success: function (response) {
              resolve(response);
          },
          error: function (error) {
              reject(error);
          },
        });
    });
}
```

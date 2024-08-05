## JavaScript: AJAX
### AJAX: Get File Data
```
// Get file data
function getFileData(filePath) {
    var xmlhttp = new XMLHttpRequest();

    xmlhttp.onreadystatechange = function () {
        if (xmlhttp.status === 200 && xmlhttp.readyState === 4) {
            var content = marked(xmlhttp.responseText);
            document.getElementById('content').innerHTML = content;
        } else {
            document.getElementById('content').innerHTML = "Error: AJAX error or no file";
        }
    };

    xmlhttp.open("GET", filePath, true);
    xmlhttp.send();
}
```

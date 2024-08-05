### JSON: Stringify
```
      var results = [];

    results.push({
        fundingId: 1,
        projectCode: 'MDEwMTAw',
        taskCode: 'MTAwNDQ1',
        defaultFunding: 1,
        fundingDescription: 'MDEwMTAwLzEwMDQ0NQ==',
        fundingSourceRemove: 0
    });

    console.log(JSON.stringify(results));
```
Result:
```
    [{
        "fundingId":1,
        "projectCode":"MDEwMTAw",
        "taskCode":"MTAwNDQ1",
        "defaultFunding":1,
        "fundingDescription":"MDEwMTAwLzEwMDQ0NQ==",
        "fundingSourceRemove":0
    }]
```
### JSON: Valid JSON has to have double quotes
Example

```
    {
      "modules": [{
        "application": 309,
        "role": "System Admin"
      }]
    }
```
### JSON: Links
* [JSON Validator](https://jsonlint.com/)
* [Comments are not allowed in JSON](https://stackoverflow.com/questions/244777/can-comments-be-used-in-json)
* [JSON {} With OpenAI](https://dev.to/mattlewandowski93/json-with-openai-3je9)

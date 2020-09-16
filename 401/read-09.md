
## Mongo population

Populated paths are no longer set to their original _id , their value is replaced with the mongoose document returned from the database by performing a separate query before returning the results.

Arrays of refs work the same way. Just call the populate method on the query and an array of documents will be returned in place of the original _ids.


## What is a Subdocument?

Subdocuments are similar to normal documents. Nested schemas can have middleware, custom validation logic, virtuals, and any other feature top-level schemas can use. The major difference is that subdocuments are not saved individually, they are saved whenever their top-level parent document is saved.

### Several types of parameters

1. **Path parameters:**
are part of the endpoint itself and are not optional. For example, in the following endpoint, {user} and {bicycleId} are required path parameters:

```javascript
/service/myresource/user/{user}/bicycles/{bicycleId}
```

2. **Query string parameters**

Query string parameters appear after a question mark (?) in the endpoint. The question mark followed by the parameters and their values is referred to as the “query string.”

```js
/surfreport/{beachId}?days=3&units=metric&time=1400
```
3. **Request bodies**
Frequently, with POST requests (where you’re creating something), you submit a JSON object in the request body. This is known as a request body, and the format is usually JSON. T

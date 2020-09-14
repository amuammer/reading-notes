# Read 08

## Discussion

#### Name 3 real world use cases where you’d want to change the request with custom middleware
1. method override
2. check auth <br/>
3. logger <br/>
4. cors

#### True or false: The route handler is middleware?
**True**

#### In what ways can a middleware function end the process and send data to the browser?
**res.download()** Prompt a file to be downloaded.<br/>
**res.end()** End the response process. <br/>
**res.json()** Send a JSON response. <br/>
**res.jsonp()** Send a JSON response with JSONP support. <br/>
**res.redirect()** Redirect a request. <br/>
**res.render()** Render a view template. <br/>
**res.send()** Send a response of various types. <br/>
**res.sendFile()** Send a file as an octet stream. <br/>
**res.sendStatus()** Set the response status code and send its string representation as the response body. <br/>

#### At what point in the request lifecycle can you “inject” middleware?
any where in the request cycle before send the response res.method();

#### What can cause express to error with “Request headers sent twice, cannot start a second response”
when you send another response for the same request. `can't set header`

## Document the following Vocabulary Terms
**Middleware** : functions that have access to the request object (req), the response object (res), and the next middleware function in the - application’s request-response cycle. <br/>

**Request Object** : the values that the client passed to the server during an HTTP request and other info related to the client.

**Response Object** : its a carrier during the request-response lifecycle, will be sent lastly to the client after finished the lifecycle.

**Application Middleware** : software that provides services beyond those provided by the operating system to enable the various components of a distributed system to communicate and manage data.

**Routing Middleware** : determining how an application responds to a client request to a particular endpoint.

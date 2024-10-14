##### GET
- status 200
- Correct data return
##### POST
- Create and check via GET
- Send with incorect / empty payload
##### PUT
- repeated requests are returned the same response
- check PUT via GET
- Send with incorect / empty payload
##### PATCH
- valid status 2xx
- Send with incorect / empty payload
##### DELETE
- POST > GET > DELETE > GET = 404
- Send to incorect object
##### HEAD
- resource is avaialble
- check HTTP header
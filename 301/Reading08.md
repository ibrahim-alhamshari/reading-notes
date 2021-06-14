## 1- What does REST stand for?
- REST is an architectural style for building distributed systems based on hypermedia.

## 2- REST APIs are designed around a __resources__.


## 3- What is an identifer of a resource? Give an example.
- It is a URI that uniquely identifies that resource. For example, the URI for a particular customer order might be:
`https://adventure-works.com/orders/1`

## 4- What are the most common HTTP verbs?
- The most common operations are GET, POST, PUT, PATCH, and DELETE

## 5- What should the URIs be based on?
- should be based on nouns (the resource) and not verbs (the operations on the resource).

## 6- Give an example of a good URI.
`https://adventure-works.com/orders`

## 7- What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?
- Web APIs that expose a large number of small resources.
- It's a bad thing.

## 8- What status code does a successful GET request return?
- returns HTTP status code 200 (OK)

## 9- What status code does an unsuccessful GET request return?
* return 404 (Not Found)

## 10- What status code does a successful POST request return?
- If a POST method creates a new resource, it returns HTTP status code 201 (Created). (Successful)

## 11- What status code does a successful DELETE request return?
- HTTP status code `204`, indicating that the process has been successfully handled.

## How would you match your name using RegEx?
- If we choose to put a name to the groups (using (?<foo>...)) we will be able to retrieve the group values using the match result like a dictionary where the keys will be the name of each group.

### *Resorces :*
- https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design
- https://regexr.com/
- https://medium.com/factory-mind/regex-tutorial-a-simple-cheatsheet-by-examples-649dc1c3f285
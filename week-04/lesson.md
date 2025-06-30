# Week 04: Postman Variables & Chaining

## Topics Covered
- Environment, Global, and Collection variables
- Setting variables in test scripts
- Using variables in request URLs and bodies
- Chaining data between requests

## Challenge

1. Send a POST request to `https://jsonplaceholder.typicode.com/posts` with the following body:

```json
{
  "title": "Postman Test",
  "body": "Learning variables!",
  "userId": 99
}
```

2. In the Tests tab, extract the `id` value from the response and save it to an environment variable called `newPostId`.

```javascript
const jsonData = pm.response.json();
pm.environment.set("newPostId", jsonData.id);
```

3. Send a GET request to `https://jsonplaceholder.typicode.com/posts/{{newPostId}}`.

4. Write tests to confirm the returned post has the correct `title` and `userId`.


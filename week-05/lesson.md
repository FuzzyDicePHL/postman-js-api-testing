# Week 05: Conditional Logic in Postman Tests

## Topics Covered
- Using if/else and logical conditions in test scripts
- Handling optional or dynamic fields
- Asserting presence of fields only if certain conditions are met

## Challenge

1. Make a request to `https://jsonplaceholder.typicode.com/comments?postId=1`
2. Write tests to:
   - Confirm the response is an array
   - Validate that each comment has a non-empty email
   - If the comment includes a `name`, ensure it is a string of at least 3 characters

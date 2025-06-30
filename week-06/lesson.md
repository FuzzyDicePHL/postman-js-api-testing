# Week 06: Chaining Requests (Data-Driven Testing)

## Topics Covered
- Passing data between requests
- Setting environment variables from one response
- Using variables in follow-up requests
- Simulating user flows across multiple API endpoints

## Challenge

1. Use `https://jsonplaceholder.typicode.com/users/1` to get a user
2. Save `username` to an environment variable (`currentUsername`)
3. Send a GET request to `https://jsonplaceholder.typicode.com/posts?userId=1`
4. Validate that each returned post includes a `title` and `body`
5. Bonus: Write a pre-request script to log the value of `currentUsername`

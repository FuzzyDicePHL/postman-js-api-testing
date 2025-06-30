# Week 07: Pre-request Scripts

## Topics Covered
- What are pre-request scripts?
- How to set headers, tokens, and timestamps before requests
- Using JavaScript in the Pre-request Script tab
- Generating dynamic values like UUIDs or timestamps

## Challenge

1. In a request to `https://jsonplaceholder.typicode.com/posts`, use a pre-request script to:
   - Generate a timestamp and save it as `requestTime`
   - Set a dynamic header `X-Request-Time` with that value

2. In the Tests tab, validate that `X-Request-Time` was sent using `pm.request.headers`

3. (Bonus) Generate a random string and send it as part of the request body

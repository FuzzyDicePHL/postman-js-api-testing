# Week 08: Using External Libraries in Postman

## Topics Covered
- Postman's built-in libraries: Lodash, Moment.js, and CryptoJS
- Practical use of Lodash for data manipulation
- Using Moment.js for time comparisons and formatting
- Using CryptoJS for hashing (e.g., SHA256)

## Challenge

1. Make a request to `https://jsonplaceholder.typicode.com/users`
2. In the **Tests tab**, use Lodash to:
   - Find the user with the longest name
   - Count how many users have email addresses from `.biz` domains
3. Use Moment.js to:
   - Log the current timestamp
   - Check if current time is within a specific range (e.g., working hours)
4. (Bonus) Generate a SHA256 hash from a fixed string using CryptoJS

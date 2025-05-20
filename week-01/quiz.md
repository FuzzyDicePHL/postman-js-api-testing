📘 Week 01 Quiz: The Basics

🧠 Multiple Choice (Answer with A, B, C, or D)

⸻

1. What does pm.test() do in Postman?
A) Executes a pre-request script
B) Sends a request
C) Defines a test case
D) Validates collection structure

⸻

2. Which of the following is the correct way to check if the response status is 200?
A) pm.expect(pm.status).to.equal(200)
B) pm.response.status(200)
C) pm.response.to.have.status(200)
D) assert.status(200)

⸻

3. What does pm.response.json() return?
A) A raw string of the response
B) A parsed JSON object
C) A list of request parameters
D) A collection of tests

⸻

4. What assertion library does Postman use behind the scenes for pm.expect()?
A) Mocha
B) Jest
C) Chai
D) Jasmine

⸻

5. Where should test scripts be written in Postman?
A) Authorization tab
B) Body tab
C) Pre-request Script tab
D) Tests tab

⸻

🧪 Short Code Exercises

⸻

6. Write a test that checks if the userId in the response body equals 1.
Assume the response is from https://jsonplaceholder.typicode.com/posts/1.

⸻

7. Write a test that ensures the title field exists and is a non-empty string.

⸻

8. Write a test that fails if the response time is over 500ms (not under).

⸻

9. Bonus Challenge:
You’re testing an API and want to make sure a field called email exists in the response and includes an @ symbol.
Write the test.


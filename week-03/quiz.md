# Week 03 Quiz: Tests and Assertions in Postman

## 📋 Instructions
- Complete all questions before the next lesson.
- Questions include **multiple choice** and **short code**.

---

### 🧠 Multiple Choice

**1. What does `pm.test()` do in Postman?**

A. Runs before the request is sent  
B. Stores global variables  
C. Executes test code after a response  
D. Generates test data

---

**2. How do you check the response status is 200?**

A. `pm.response.hasStatus(200)`  
B. `pm.response.code === 200`  
C. `pm.expect(pm.response.status).to.eql(200)`  
D. `pm.response.to.have.status(200)`

---

**3. Which method parses the response body as JSON?**

A. `pm.body.parse()`  
B. `pm.expect.json()`  
C. `pm.response.json()`  
D. `JSON.parse(pm.response)`

---

### 🧑‍💻 Code Questions

**4. Write a test to check that the response time is below 300ms.**

```javascript
// Your answer here
```

---

**5. Write a test that checks if the `title` field exists and is not empty in a JSON response.**

```javascript
// Your answer here
```

---

**6. Write a test to ensure the response has a `Content-Type` header.**

```javascript
// Your answer here
```

---

✅ When complete:
- Save this file as `quiz.md` in your `week-03/` folder on GitHub.


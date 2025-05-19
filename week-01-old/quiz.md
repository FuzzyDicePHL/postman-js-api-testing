# Week 01 Quiz

Test your Week 01 knowledge — no trick questions, just good practice.

---

1. What does `pm.test()` do in Postman?  
A) Sends the API request  
B) Validates part of the response  
C) Converts the response to JSON  
D) Sets environment variables  

**Correct answer:** B

---

2. Which method checks the HTTP status code?  
A) `pm.expect.status(200)`  
B) `pm.response.checkStatus(200)`  
C) `pm.response.to.have.status(200)`  
D) `pm.response.isStatus(200)`  

**Correct answer:** C

---

3. Write a Postman test that checks the `title` field is not empty.  

```javascript
pm.test("Title is not empty", function () {
  var jsonData = pm.response.json();
  pm.expect(jsonData.title).to.not.be.empty;
});
```

---

4. What format should you use when exporting a Postman collection?  
A) Collection v1.0  
B) Postman v2  
C) Collection v2.1  
D) JSON v3  

**Correct answer:** C

---

5. BONUS: What’s the difference between `==` and `===` in JavaScript?  

**Answer:**  
`===` checks for both value and type (strict equality).  
`==` allows type coercion, so values can be equal even if their types differ.

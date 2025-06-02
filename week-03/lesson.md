# Week 03: Tests and Assertions in Postman Using JavaScript

## What You’ll Learn
This week, you’ll explore how to:
- Write **tests** using `pm.test()` in Postman
- Use **assertions** with JavaScript and Chai.js-style syntax
- Validate response data, headers, status codes, and more

---

## 🔹 1. Writing Basic Tests

Postman allows you to write tests that run after a response is received.

```javascript
pm.test("Status code is 200", function () {
  pm.response.to.have.status(200);
});
```

You can write multiple `pm.test()` functions in one request.

---

## 🔹 2. Common Assertions

Postman uses a BDD-style assertion library (Chai.js). Here are common patterns:

```javascript
// Response time
pm.test("Response time is below 500ms", function () {
  pm.expect(pm.response.responseTime).to.be.below(500);
});

// Check for a field in JSON response
pm.test("Response has userId field", function () {
  const jsonData = pm.response.json();
  pm.expect(jsonData).to.have.property("userId");
});

// Check a specific value
pm.test("userId is 1", function () {
  const jsonData = pm.response.json();
  pm.expect(jsonData.userId).to.eql(1);
});
```

---

## 🔹 3. Checking Headers

You can also verify headers like so:

```javascript
pm.test("Content-Type is JSON", function () {
  pm.response.to.have.header("Content-Type");
});
```

---

## 🧪 Practice Exercise

1. Send a `GET` request to:
   ```
   https://jsonplaceholder.typicode.com/posts/1
   ```

2. Add these tests in the **Tests** tab:

   ```javascript
   pm.test("Status code is 200", function () {
     pm.response.to.have.status(200);
   });

   pm.test("Post ID is 1", function () {
     const jsonData = pm.response.json();
     pm.expect(jsonData.id).to.eql(1);
   });

   pm.test("Title is not empty", function () {
     const jsonData = pm.response.json();
     pm.expect(jsonData.title).to.not.be.empty;
   });
   ```

3. Run the request and view results in the **Test Results** tab.

---

## 🧰 Extra Challenge

Write a test that ensures:
- Response time is under 200ms
- Response body contains the word `"sunt"` in the title

---

## Suggested GitHub Structure

```
postman-js-api-testing/
└── week-03/
    ├── lesson.md
    ├── quiz.md
    └── Lesson 03 - Writing Tests.postman_collection.json
```

Once you’ve practiced this material, move on to the quiz to confirm your knowledge.


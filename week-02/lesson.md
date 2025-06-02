# Week 02: Variables, Pre-request Scripts, and Environments

## What You’ll Learn
This week, you’ll explore how to:
- Use **Postman variables** to avoid hardcoding data.
- Set up **environments** to handle different API contexts (like dev, test, prod).
- Write **Pre-request Scripts** in JavaScript to dynamically set variables before sending a request.

---

## 🔹 1. Postman Variables

Postman allows four scopes of variables:

- **Global** – available everywhere  
- **Collection** – tied to a collection  
- **Environment** – tied to a specific environment  
- **Local** – specific to the request  

You can reference them using double curly braces:

```
{{base_url}}
```

---

## 🔹 2. Environments

Environments allow you to switch between sets of variables, useful for separating dev/test/prod.  
Create environments with variable sets like:

```json
{
  "base_url": "https://api.devsite.com",
  "auth_token": "abcdef123456"
}
```

Switch environments using the dropdown in the top-right corner of Postman.

---

## 🔹 3. Pre-request Scripts

Pre-request scripts run *before* a request is sent and are written in JavaScript.

Example: setting a random ID

```javascript
let id = Math.floor(Math.random() * 1000);
pm.environment.set("random_id", id);
```

You can use these scripts to:
- Generate tokens
- Create dynamic query strings
- Chain requests

---

## 🧪 Practice Exercise

1. Create a new environment called `Week02-Env` with these variables:
   - `base_url = https://postman-echo.com`
   - `random_id = (leave blank)`

2. Create a GET request to:
   ```
   {{base_url}}/get?id={{random_id}}
   ```

3. In the **Pre-request Script** tab, add:

   ```javascript
   let id = Math.floor(Math.random() * 1000);
   pm.environment.set("random_id", id);
   ```

4. Send the request and verify that a new random `id` appears each time in the response.

---

## 🧰 Extra Practice

Write a pre-request script that:
- Grabs the current date
- Formats it as `YYYY-MM-DD`
- Sets it as a variable called `today`

```javascript
let today = new Date().toISOString().split("T")[0];
pm.environment.set("today", today);
```

---

## Suggested GitHub Structure

```
postman-js-api-testing/
└── week-02/
    ├── lesson.md
    ├── quiz.md
    └── Lesson 02 - Variables and Scripts.postman_collection.json
```

Once you’ve practiced this material, move on to the quiz to test your knowledge.


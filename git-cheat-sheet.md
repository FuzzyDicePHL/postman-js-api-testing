
# 🧠 Git Command Cheat Sheet for Postman + JS API Testing Repo

Your current directory structure:
```
postman-js-api-testing/
├── README.md
├── lesson-1/
│   └── README.md
└── week-01/
    ├── lesson.md
    └── quiz.md
```

---

## 🧱 Basic Setup

### Initialize a repo (do this once per new project)
```bash
git init
```

### Connect your local repo to GitHub (once per repo)
```bash
git remote add origin https://github.com/FuzzyDicePHL/postman-js-api-testing.git
```

---

## 💾 Workflow: Add → Commit → Push

### See what's changed
```bash
git status
```

### Stage your changes
```bash
git add .                       # All changes
git add week-01/quiz.md         # Just one file
```

### Commit your changes
```bash
git commit -m "Add quiz for week-01"
```

### Push to GitHub
```bash
git push origin main
```

---

## 📥 Pull the latest changes from GitHub

```bash
git pull origin main
```

If you get a history conflict:
```bash
git pull origin main --allow-unrelated-histories
```

---

## 🛠️ Undo / Cleanup

### Discard changes to a file (not committed yet)
```bash
git checkout -- filename.js
```

### View commit history
```bash
git log --oneline
```

### See remote connection info
```bash
git remote -v
```

---

## 🔧 Example: Add new lesson and quiz

```bash
mkdir -p lesson-2 week-02
touch lesson-2/README.md week-02/lesson.md week-02/quiz.md
git add lesson-2/ week-02/
git commit -m "Add lesson-2 and week-02 structure"
git push origin main
```

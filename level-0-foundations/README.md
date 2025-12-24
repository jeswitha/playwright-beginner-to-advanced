# 🔰 Level 0 — Foundations (Absolute Beginner)

Welcome to **Level 0** of the *Master Test Automation with Playwright* course.

This level is designed for **absolute beginners**:
- No automation experience
- No Playwright knowledge
- Minimal or no coding background

🚫 There is **no test code** in this level  
🧠 This level focuses entirely on **mental models and understanding**

---

## 🎯 Goal of Level 0

By the end of this level, you should clearly understand:

- What software testing is
- Why automation exists
- What Playwright does (in simple terms)
- What a browser actually is from an automation point of view
- What you will be automating in later levels

If these ideas are clear, everything else becomes easier.

---

## 📘 Lesson 0.1 — What Is Software Testing?

### In simple words:
Software testing means **checking whether software behaves the way humans expect it to**.

Examples:
- Does a login button actually log you in?
- Does a payment page show success after payment?
- Does an error message appear when something goes wrong?

---

### Manual Testing vs Automated Testing

**Manual testing**
- A human clicks buttons
- A human types values
- A human checks results

**Automated testing**
- A program clicks buttons
- A program types values
- A program checks results

👉 Automation is used when:
- The same checks are repeated often
- Speed and reliability matter
- Human effort should be reduced

---

### What Problems Does Automation Solve?

Automation helps with:
- Repeating tests quickly
- Catching bugs earlier
- Running tests overnight
- Testing across multiple browsers
- Reducing human mistakes

Automation does **NOT** replace humans — it supports them.

---

## 📘 Lesson 0.2 — What Is Playwright?

### Think of Playwright like this:
> 🤖 Playwright is a robot that controls a web browser the same way a human does.

It can:
- Open a browser
- Click buttons
- Type text
- Read what appears on the screen
- Decide if something is correct or broken

---

### Why Playwright?

Playwright is chosen because:
- It supports **Chromium, Firefox, and WebKit**
- It automatically waits for things to be ready
- It is fast and reliable
- It works well for modern web apps
- It is backed by Microsoft

---

### What Is End-to-End (E2E) Testing?

E2E testing means:
- Starting from the user’s first action
- Ending at the final result

Example:

Playwright is mainly used for **E2E testing**.

---

## 📘 Lesson 0.3 — How the Web Works (Mental Model)

### What Is a Website?
A website is a collection of files:
- HTML → structure
- CSS → appearance
- JavaScript → behavior

---

### What Is a Browser?
A browser:
- Downloads website files
- Displays them
- Runs JavaScript
- Lets users interact with pages

Automation tools like Playwright **control the browser**, not the server.

---

### What Automation Actually Controls

Playwright does NOT:
- Change backend logic
- Modify databases directly

Playwright DOES:
- Interact with buttons, links, inputs
- Read text and UI state
- Simulate real user behavior

---

## ✅ When Are You Ready to Move to Level 1?

You are ready for Level 1 if:
- You understand what automation is
- You know what Playwright does
- You are comfortable moving to setup and installation

👉 If not, **re-read this level slowly**. That’s normal.

---

➡️ Next: **Level 1 — Environment Setup & Playwright Basics**

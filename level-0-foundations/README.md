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

=================================================================
>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
//////////////////////////////////////////////////////////////////

0.1 What Is Software Testing?

Non-technical mental model

Software testing is like checking a new house before you move in:

Does the door lock?

Does the tap work?

Does the light switch actually turn on the light?

If something is wrong, does the house warn you (leak alarm) instead of silently failing?

Testing = checking behavior matches expectations.

Technical mental model

Testing is the process of verifying a system:

Does what it should do (requirements/user expectations)

Doesn’t do what it shouldn’t do (security, invalid inputs)

Keeps doing it consistently after changes (regression)

What you validate in software

Functionality: feature works (login, checkout)

Usability: easy to use, clear messages

Reliability: doesn’t randomly fail

Performance: responds fast enough

Security: protects user/data

Compatibility: works on browsers/devices

Memory hook

Testing = “Expectation vs Reality.”
If expectation and reality match → pass. If not → bug.

Mini exercise (30 seconds)

Pick any app you use daily (Amazon, Gmail, Instagram).
Write 3 expectations like:

“If I type wrong password, I should see an error.”

“If I search, results should appear.”

“If I click logout, I should be logged out.”

That’s testing.

0.2 Manual Testing vs Automated Testing

Manual testing (non-technical)

Manual testing is like tasting food while cooking:

You taste, adjust, taste again

Great for creativity, exploration, and catching “weirdness”

Automated testing (non-technical)

Automation is like using a rice cooker:

Once set up correctly, it repeats perfectly every time

Doesn’t get tired, doesn’t forget steps

Technical differences

Manual

Best for: new features, exploratory testing, UI feel, edge cases discovery

Weakness: slow, inconsistent, expensive for repetition

Automation

Best for: regression, repeated checks, high frequency flows, CI/CD

Weakness: initial setup cost, maintenance, cannot “feel” usability

Big truth (important)

Automation does not replace humans.
It replaces repetition, not thinking.

Memory hook

Humans are best at finding new problems.
Automation is best at preventing old problems from returning.

0.3 Why Automation Exists (What Problems It Solves)

What automation solves (non-technical)

Imagine you own a restaurant and every day you must check:

fridge temp

gas leak

fire alarm

door lock

Doing it manually daily is exhausting.
So you install sensors/alarms to check automatically.

Automation is that “sensor system” for your software.

Technical reasons automation exists

Regression: new code breaks old features

Speed: run hundreds/thousands of checks quickly

Consistency: same steps every run

Coverage: multiple browsers/devices

Shift-left: catch issues earlier in pipeline

Confidence: releases become safer/faster

What automation does NOT solve

Bad requirements

Poor UX decisions

Missing product clarity

“This feels confusing” issues

All bugs (it finds the bugs you teach it to check)

Memory hook

Automation is confidence at scale.

0.4 What Is Playwright?
Non-technical definition

Playwright is a browser robot:

It opens a browser

clicks, types, scrolls

reads what’s on screen

checks if the app behaved correctly

Technical definition

Playwright is an end-to-end browser automation framework that:

Uses browser engines (Chromium/Firefox/WebKit)

Controls pages via automation protocols

Provides test runner + assertions + fixtures (when using Playwright Test)

Has auto-waiting and strong reliability features

What Playwright can automate

UI actions: click/type/select/upload

navigation and routing

waiting for UI/network events

validations: text, visibility, URL, element state

screenshots/video/trace debugging

Why Playwright is popular

Cross-browser support

Auto-waits reduce flakiness

Fast parallel execution

Great debugging (traces)

Works well in CI

Memory hook

Playwright = Driver + Brain
Driver controls browser. Brain decides pass/fail (assertions).

0.5 End-to-End (E2E) Testing
Non-technical

E2E is like testing a full “customer journey”:

enter store → choose items → pay → get receipt → leave happy

Not just “cart works” or “payment API works” alone.

Technical

E2E validates a full user workflow across components:

UI + frontend logic

APIs

backend services (indirectly)

integrations (auth, payment, etc.)

Example E2E flow:
Login → Search product → Add to cart → Checkout → Confirm order

Strengths

Highest confidence (closest to real user)

Catches integration issues

Weaknesses

Slower than unit/API tests

More brittle than lower-level tests

Needs stable environments/test data

Memory hook

Unit tests = single brick
API tests = wall section
E2E tests = entire house walkthrough

0.6 How a Website Works (Mental Model)
Non-technical

A website is like a stage show:

HTML = stage structure (walls, doors)

CSS = costumes/lighting (how it looks)

JavaScript = actors + actions (what happens when you click)

Technical

HTML (DOM): defines elements (buttons, inputs)

CSS: styles elements (color, layout)

JavaScript: updates DOM, calls APIs, handles events

When you open a site:

browser downloads HTML/CSS/JS

builds DOM

applies CSS

runs JS

user interacts → JS reacts → UI updates + API calls

Memory hook

HTML = what it is
CSS = how it looks
JS = what it does

0.7 What a Browser Does vs What Automation Controls
What a browser does (technical)

Requests resources from servers (HTTP)

Renders DOM + CSS

Runs JS engine

Manages cookies/session/storage

Handles user events (clicks, typing)

What Playwright controls

Playwright controls the browser context and page:

click/type/hover/scroll

read DOM/text/state

intercept network (mock/stub)

manage cookies/storage

run JS in page context

What Playwright does NOT do directly

It doesn’t “edit the database” directly

It doesn’t rewrite backend logic

It can’t magically fix broken requirements

But it can:

Trigger backend changes through the UI/API like a real user would

Validate results shown in UI

Memory hook

Playwright controls what the user can touch.

0.8 Readiness to Move to Level 1

You’re ready for Level 1 if you can explain these in one sentence each:

Testing: checking expected vs actual behavior

Automation: code repeating checks consistently

Playwright: a tool that controls browsers like a user

E2E: testing full user journeys end-to-end

Browser vs server: browser renders + runs JS; Playwright controls browser interactions

Quick self-check (answer in your head)

Why do we automate regression tests?

What does Playwright control: server or browser?

What are HTML/CSS/JS responsible for?

If you can answer those, Level 1 will feel easy.

-----------------------------------------------------

Your “Never Forget” Practice (2 minutes)

Do this once and you’ll remember forever:

Take a simple flow: Login

Manual testing: “I type username/password and click login”

Automation: “A script types username/password and clicks login”

E2E: “Login → land on dashboard → verify username shown”

Website model: HTML input + CSS style + JS sends API request

Browser vs Playwright: browser renders; Playwright clicks/types/reads

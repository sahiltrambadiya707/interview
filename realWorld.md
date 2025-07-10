---

# 💼 Real-Life Scenario-Based Interview Questions

Grouped by:

* 👷 Full-stack App Development
* ⚛️ React.js Scenarios
* 🌐 Node.js / API Layer
* 🚀 MongoDB & Data Modeling
* 🔄 DevOps / CI / Production
* 🔐 Auth & Security
* 💬 Team & Collaboration

---

## 👷 Full-Stack Project Scenarios

| Difficulty | Question                                                                                                                                           |
| ---------- | -------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🟡         | You're building a dashboard with 5+ widgets that each make API calls. How would you structure your API to minimize load time and network requests? |
| 🔴         | You’re assigned to refactor a monolith into microservices. What’s your approach to splitting it while avoiding breaking existing features?         |
| 🟡         | In a multi-tenant app, how do you manage per-tenant DB schemas or access? How do you isolate tenant data?                                          |
| 🔴         | You’re working on a real-time stock dashboard. How do you sync updates to thousands of users without flooding the server?                          |
| 🔴         | Your product manager says, "The app is slow!" — how do you diagnose what’s slow: frontend, backend, DB, or network?                                |

---

## ⚛️ React.js Scenario Questions

| Difficulty | Question                                                                                                                                       |
| ---------- | ---------------------------------------------------------------------------------------------------------------------------------------------- |
| 🟡         | You have a React app with a lot of prop drilling. Redux feels overkill. What are alternative patterns you’d implement?                         |
| 🔴         | A component re-renders on every keystroke, even though data hasn't changed. How do you optimize performance?                                   |
| 🔴         | You’re integrating a complex form with dynamic fields, conditional validation, and multilingual support. How would you design the form system? |
| 🟡         | You’re using `useEffect` to fetch data but it’s firing multiple times. What could be wrong and how do you fix it?                              |
| 🔴         | Explain how you would lazy-load heavy components and animations in a multi-tab dashboard without hurting UX.                                   |

---

## 🌐 Node.js / API Architecture

| Difficulty | Question                                                                                                                      |
| ---------- | ----------------------------------------------------------------------------------------------------------------------------- |
| 🟡         | Your API must support both public and admin users. How do you implement role-based access without duplicating route logic?    |
| 🔴         | You need to run webhook calls **in order per tenant**, even though requests come in parallel. How would you handle this?      |
| 🟡         | How do you handle API versioning in a growing backend with legacy and new clients?                                            |
| 🔴         | A user triggers an expensive DB operation. How would you move it to background processing while returning a success response? |
| 🟡         | You want to keep your Express code modular and testable. How do you structure routes, controllers, and services?              |

---

## 🚀 MongoDB & Schema Design

| Difficulty | Question                                                                                                                              |
| ---------- | ------------------------------------------------------------------------------------------------------------------------------------- |
| 🟡         | You need to design a schema for user portfolios with nested assets and trades. How would you balance performance vs. flexibility?     |
| 🔴         | You’re hitting performance issues on a collection with 10M+ documents. How do you use indexes to optimize search?                     |
| 🔴         | You want to support flexible filters, sorting, and pagination in a complex table. How do you dynamically build the aggregation query? |
| 🟡         | How would you store dynamic form responses for different clients, while maintaining validation and searchability?                     |
| 🔴         | You need to deduplicate `$lookup` in aggregation pipelines when building queries dynamically. How do you handle that?                 |

---

## 🔄 DevOps / CI / Production

| Difficulty | Question                                                                                                          |
| ---------- | ----------------------------------------------------------------------------------------------------------------- |
| 🟡         | How do you set up environment-specific config (dev, staging, prod) in a full-stack app using .env?                |
| 🔴         | A new release broke your app in production. How do you roll back safely and identify the root cause?              |
| 🟡         | Your frontend needs `.env` secrets at build time. How do you expose only what’s needed and secure sensitive ones? |
| 🔴         | You deploy multiple containers for Node.js API. How do you ensure logs are aggregated and readable for debugging? |

---

## 🔐 Auth & Security

| Difficulty | Question                                                                                                       |
| ---------- | -------------------------------------------------------------------------------------------------------------- |
| 🟡         | How do you manage user sessions in a React + Node app — JWT vs cookie-based auth?                              |
| 🔴         | You're storing refresh tokens in MongoDB but users report getting logged out randomly. What could go wrong?    |
| 🟡         | How do you prevent CSRF and XSS in a React + Express app?                                                      |
| 🔴         | You’re implementing 2FA. How would you design the flow including device trust, backup codes, and token expiry? |
| 🔴         | How would you protect file uploads from executable malware and secure the image CDN?                           |

---

## 💬 Team & Collaboration

| Difficulty | Question                                                                                                     |
| ---------- | ------------------------------------------------------------------------------------------------------------ |
| 🟡         | You’re handed an unfamiliar codebase with zero documentation. What are your first steps?                     |
| 🟡         | A teammate insists on rewriting a working feature. How do you approach the discussion?                       |
| 🔴         | You're asked to mentor a junior dev who's struggling with async logic. How do you coach them with examples?  |
| 🔴         | Your team has slow code reviews. What systems would you introduce to improve speed without lowering quality? |

---


Here’s a set of **tool-specific interview questions** grouped by:

* 🔧 **Version Control** (Git)
* 🧠 **Editors & IDEs** (VS Code, WebStorm)
* 📦 **Package Managers** (NPM, Yarn, pnpm)
* 📘 **Documentation & UI Tools** (Storybook)
* 🧪 **Testing Tools** (Jest, Cypress – optional bonus)
* 📚 **Bonus: Dev Tools & Linting** (ESLint, Prettier, Browsers)

---

# 🔧 Tooling-Based Interview Questions

Each marked with difficulty:
🟢 Basic 🟡 Mid 🔴 Expert

---

## 🧱 Git (Version Control)

| Difficulty | Question                                                                                                |
| ---------- | ------------------------------------------------------------------------------------------------------- |
| 🟢         | What is the difference between `git pull` and `git fetch`?                                              |
| 🟢         | How do you revert the last commit without losing changes?                                               |
| 🟡         | How do you squash multiple commits into one?                                                            |
| 🟢         | What does `git stash` do? How do you apply and drop a stash?                                            |
| 🔴         | You’ve accidentally pushed secrets to the remote repo. How do you permanently remove them from history? |
| 🟡         | Explain `rebase` vs `merge`. When would you use each?                                                   |
| 🔴         | What is a Git hook? How do you use one for pre-commit linting or formatting?                            |
| 🟢         | How do you resolve merge conflicts? What’s your typical workflow?                                       |
| 🔴         | What’s the difference between `git reflog` and `git log`? When would you use `reflog`?                  |
| 🟡         | How would you handle versioning and release tagging in a monorepo?                                      |

---

## 🧠 VS Code / IDEs

| Difficulty | Question                                                                            |
| ---------- | ----------------------------------------------------------------------------------- |
| 🟢         | How do you search across all files in a VS Code project?                            |
| 🟢         | What are some VS Code extensions you always install for React/Node development?     |
| 🟡         | How do you configure VS Code to auto-format code on save (with Prettier or ESLint)? |
| 🔴         | How would you debug an Express API using breakpoints in VS Code?                    |
| 🟢         | How do you open VS Code in a specific folder from terminal?                         |
| 🟡         | What is the difference between workspace settings and global settings in VS Code?   |
| 🔴         | Have you ever used multi-root workspaces in VS Code? What’s the use case?           |

---

## 📦 NPM / Yarn / pnpm

| Difficulty | Question                                                                                        |
| ---------- | ----------------------------------------------------------------------------------------------- |
| 🟢         | What is the difference between `dependencies` and `devDependencies`?                            |
| 🟢         | What is a `package-lock.json` and why is it important?                                          |
| 🟡         | When should you use `--save-exact` during installation?                                         |
| 🟡         | How does `npx` differ from `npm`? Give a real-world use case.                                   |
| 🔴         | How does Yarn Plug'n'Play work? What are its pros and cons?                                     |
| 🔴         | What are workspaces in Yarn or pnpm? How do they help in monorepos?                             |
| 🟢         | What’s the purpose of using `.npmrc`? What’s one key you’ve configured in it?                   |
| 🟡         | You run `npm install` and it breaks. How do you debug or clean the install?                     |
| 🔴         | How would you publish a custom npm package securely? What files should be included or excluded? |

---

## 📘 Storybook.js

| Difficulty | Question                                                                                |
| ---------- | --------------------------------------------------------------------------------------- |
| 🟢         | What is Storybook and why would you use it?                                             |
| 🟡         | How do you write a basic Storybook story for a Button component?                        |
| 🔴         | How would you use controls and decorators to make stories more interactive and dynamic? |
| 🟡         | How does Storybook help in building design systems?                                     |
| 🔴         | Can you integrate Storybook into a CI pipeline for visual regression testing? How?      |
| 🔴         | How do you organize stories in a scalable component library?                            |
| 🟡         | What addons have you used with Storybook and why (e.g., knobs, actions, viewport)?      |

---

## 🧪 (Optional Bonus) — Testing Tools

| Difficulty | Question                                                                      |
| ---------- | ----------------------------------------------------------------------------- |
| 🟢         | What’s the difference between unit testing and integration testing?           |
| 🟡         | How do you mock API responses in Jest or MSW?                                 |
| 🔴         | How would you integrate Cypress with CI/CD for full e2e testing?              |
| 🔴         | How do you write a test for a dynamic React component with hooks and context? |

---

## 💅 Bonus: ESLint, Prettier, Browsers

| Difficulty | Question                                                                                         |
| ---------- | ------------------------------------------------------------------------------------------------ |
| 🟡         | How do you enforce consistent formatting using Prettier across your team?                        |
| 🔴         | How do you override ESLint rules for a specific file or line?                                    |
| 🔴         | You’re debugging CORS issues in the browser. What tools do you use to isolate and fix it?        |
| 🔴         | How do you analyze bundle size and reduce TTI (Time To Interactive) in a production React build? |

---

# 🧼 GitHub Hygiene & Git Best Practices
> A comprehensive guide to maintaining clean, secure, and professional repositories.

---

## 1. ✍️ Master the Commit Message
A commit is a snapshot in time. The message should explain **why** a change was made, not just **what** was changed.

### The "Golden Rules" of Commits:
* **Use the Imperative Mood:** Write the message as if you are giving a command to the codebase.
    * ❌ *Bad:* "I fixed the broken link"
    * ✅ *Good:* "Fix broken link in footer"
* **Be Concise but Descriptive:** Aim for 50 characters or less for the subject line.
* **No "Junk" Commits:** Avoid messages like "update," "test," or "fixing stuff."

| Action | Professional Message Example |
| :--- | :--- |
| Adding a feature | `Add user authentication logic` |
| Fixing a bug | `Fix alignment issue on mobile navigation` |
| Updating docs | `Update README with installation steps` |
| Refactoring | `Refactor database query for better performance` |

---

## 2. 🛡️ Security & Data Protection
GitHub is a public stage. Once sensitive data is pushed, it is very difficult to "un-ring" the bell.

### Critical Security Rules:
* **Never Push Secrets:** Do not hardcode API keys, passwords, or tokens directly into your code.
* **Use Environment Variables:** Store secrets in a `.env` file on your local machine.
* **The "Point of No Return":** If you accidentally push a password, **change the password immediately**. Deleting the commit is not enough because it remains in the Git history.

---

## 3. 🚫 The Power of `.gitignore`
The `.gitignore` file tells Git which files to stay away from. This keeps your repository lightweight and secure.

### What should stay out of your Repo?
* **System Files:** `.DS_Store` (Mac) or `Thumbs.db` (Windows).
* **Dependencies:** `node_modules/` or `venv/` (These are huge folders that can be re-installed via a command).
* **Sensitive Files:** `.env` (Your API keys).
* **Temporary Files:** Logs, cache, and build folders like `dist/` or `out/`.

**Example `.gitignore` content:**
```text
.env
.DS_Store
node_modules/
*.log


A professional repo should be "self-documenting." Anyone landing on your page should understand the project within 30 seconds.

The "Clean Repo" Checklist:

The README.md: The "front door" of your project. Must include a title, description, and setup instructions.

Folder Hierarchy: * /src — All your logic and code.

/assets — Images, icons, and CSS.

/docs — Additional guides or manuals.

License File: Always choose a license (like MIT) so others know how they can use your work.

Keep it Current: Delete "dead" branches once they are merged into the main project.

### How to use this:
1.  **In VS Code**, click the "New File" icon in your explorer sidebar.
2.  Name it `HYGIENE.md`.
3.  **Paste** the content above.
4.  **Commit and Push** it just like you did with your journal entries.


[⬅️ Back to Main Journal](./README.md)

# 🐞 Bug Report: Product Images match incorrect source

| Field | Description |
|---|---|
| **Bug ID** | BUG-001 |
| **Title** | Product images on Inventory page are displayed as placeholders (dog image) for "problem_user" |
| **Severity** | **Major** (UI issue affecting user experience and product presentation) |
| **Priority** | **High** |
| **Status** | Open |
| **Author** | QA Engineer |
| **Date** | 2025-12-16 |

---

### 💻 Environment
* **URL:** https://www.saucedemo.com/inventory.html
* **Browser:** Google Chrome (Version 120.0)
* **OS:** Windows 10 / macOS
* **Test Data:** Username: `problem_user` / Password: `secret_sauce`

### 📝 Description
When logging in with the specific "problem_user" account, all product images on the inventory listing page are replaced with the same placeholder image (a dog), failing to show the actual product visuals.

### 👣 Steps to Reproduce
1.  Navigate to https://www.saucedemo.com/
2.  Enter username `problem_user`.
3.  Enter password `secret_sauce`.
4.  Click the **"Login"** button.
5.  Observe the images next to each product name (e.g., Sauce Labs Backpack).

### ✅ Expected Result
Each product should display its specific corresponding image (e.g., a backpack for "Sauce Labs Backpack").

### ❌ Actual Result
All product images are identical (displaying a picture of a dog) and do not match the product description. `src` attribute is likely broken or redirected.

---
**Attachments:**
*(In a real Jira ticket, a screenshot would be attached here showing the dog images)*

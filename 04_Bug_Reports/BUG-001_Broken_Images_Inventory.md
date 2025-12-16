# 🐞 Bug Report: Wrong Images for "problem_user"

| Field | Description |
|---|---|
| **ID** | BUG-001 |
| **Title** | All products show the same "Dog" image instead of real photos for `problem_user` |
| **Severity** | **Major** (Users cannot see what they are buying) |
| **Priority** | **High** |
| **Status** | Open |
| **Date** | 2025-12-16 |

---

### 💻 Environment
* **Website:** https://www.saucedemo.com/inventory.html
* **Browser:** Chrome (Latest version)
* **Account:** `problem_user` / `secret_sauce`

### 📝 What is the problem?
When I log in as the `problem_user`, the product photos are broken. Every item (Backpack, Bike Light, etc.) shows the same picture of a dog instead of the real product photo.

### 👣 Steps to reproduce
1. Go to https://www.saucedemo.com/
2. Type username `problem_user`.
3. Type password `secret_sauce`.
4. Click **Login**.
5. Look at the product images.

### ✅ Expected Result
I should see the correct photo for each item (e.g., a picture of a Backpack for the "Sauce Labs Backpack").

### ❌ Actual Result
All items show the same "Dog" image. The correct photos do not load.

---
**Attachments:**
*(In a real report, I would add a screenshot of the dog images here)*

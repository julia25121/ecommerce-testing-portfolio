# 📋 Test Plan: Swag Labs

**Project:** Swag Labs Online Store
**Version:** 1.0
**Author:** Manual QA Engineer

---

## 1. Introduction
The goal of this plan is to test the main functions of the **Swag Labs** (SauceDemo) website. I want to make sure that users can log in, choose products, and buy them without errors.

## 2. Scope (What to test)

### ✅ What I will test
I will focus on these main features:

1.  **Login / Logout:**
    * Logging in with correct and wrong passwords.
    * Checking what happens with blocked users.
    * Logging out.
2.  **Product List (Inventory):**
    * Viewing products.
    * Sorting items (by Price or Name).
    * Adding and removing items from the Cart.
3.  **Shopping Cart:**
    * Checking if the correct items are in the cart.
    * Button "Continue Shopping".
4.  **Checkout (Buying):**
    * Checking the form (First Name, Last Name, Zip Code).
    * Checking the total price and tax.
    * Finishing the order ("Thank you" page).

### ❌ What I will NOT test
* **Performance:** I am not checking how fast the site works under heavy load.
* **Security:** I am not testing for hacking vulnerabilities (like SQL Injection).
* **API:** I am testing only the User Interface (UI), not the backend code.
* **Mobile App:** I am testing the website in the browser, not a mobile application.

## 3. Test Strategy
* **Type:** Manual Testing (Black Box).
* **Browsers:** Chrome (Latest version) and Firefox.
* **Test Data:** I will use the standard accounts provided by the site (`standard_user`, `problem_user`, etc.).

## 4. When to start and stop?
* **Entry Criteria (Start):** The website https://www.saucedemo.com/ is working and opens in the browser.
* **Exit Criteria (Stop):** All important tests (Checkout flow) are done, and major bugs are reported.

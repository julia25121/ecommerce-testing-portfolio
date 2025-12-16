# 📋 Master Test Plan: Swag Labs

**Project:** Swag Labs E-commerce Website  
**Version:** 1.0  
**Author:** Manual QA Engineer  

---

## 1. Introduction
The objective of this Test Plan is to define the scope, approach, and resources required for functional testing of the **Swag Labs** (SauceDemo) web application. The focus is on verifying core business flows for different user roles.

## 2. Scope of Testing

### ✅ In Scope 
The following features will be tested functionally:
1.  **Authentication:**
    * Login with valid/invalid credentials.
    * Login with locked-out users.
    * Logout functionality.
2.  **Inventory (Product Catalog):**
    * Viewing products.
    * Sorting functionality (Name A-Z, Price Low-High).
    * Adding/Removing items to Cart.
3.  **Shopping Cart:**
    * Verifying added items.
    * "Continue Shopping" navigation.
4.  **Checkout Process:**
    * Information form validation (First Name, Last Name, Zip).
    * Overview page verification (Item total + Tax calculation).
    * Order completion ("Thank you" page).

### ❌ Out of Scope 
* **Performance Testing:** Load and Stress testing are not part of this iteration.
* **Security Testing:** SQL Injection or Penetration testing.
* **API Testing:** Backend verification is out of scope for this manual run.
* **Mobile App:** We are testing the responsive web version, not native mobile apps.

## 3. Test Strategy
* **Test Type:** Manual Black-Box Testing.
* **Browsers:** Google Chrome (Latest Version), Firefox.
* **Test Data:** Used provided test accounts (`standard_user`, `problem_user`, `locked_out_user`).

## 4. Entry & Exit Criteria
* **Entry Criteria (Start):** The website https://www.saucedemo.com/ is accessible.
* **Exit Criteria (Stop):** All critical test cases (Checkout flow) are executed. Major bugs are reported.

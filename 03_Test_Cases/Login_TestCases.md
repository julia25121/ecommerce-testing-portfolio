# 🔐 Test Suite: User Login

**Module:** Authentication  
**Tested URL:** https://www.saucedemo.com/  
**Test Data:** - Valid User: `standard_user`
- Locked User: `locked_out_user`
- Password: `secret_sauce`

---

| TC ID | Title | Pre-conditions | Test Steps | Expected Result | Priority |
|---|---|---|---|---|---|
| **TC-LGN-001** | **Successful Login (Standard User)** | User is on the Login page | 1. Enter valid username (`standard_user`).<br>2. Enter valid password (`secret_sauce`).<br>3. Click "Login" button. | User is redirected to the "Inventory" page (`/inventory.html`). Product list is visible. | High |
| **TC-LGN-002** | **Login with Invalid Password** | User is on the Login page | 1. Enter valid username (`standard_user`).<br>2. Enter **invalid** password (e.g., `12345`).<br>3. Click "Login" button. | Error message is displayed: *"Epic sadface: Username and password do not match any user in this service"*. User remains on Login page. | High |
| **TC-LGN-003** | **Login with Locked Out User** | User is on the Login page | 1. Enter locked username (`locked_out_user`).<br>2. Enter valid password (`secret_sauce`).<br>3. Click "Login" button. | Error message is displayed: *"Epic sadface: Sorry, this user has been locked out."*. User is not logged in. | Medium |
| **TC-LGN-004** | **Login with Empty Fields** | User is on the Login page | 1. Leave Username field empty.<br>2. Leave Password field empty.<br>3. Click "Login" button. | Error message is displayed: *"Epic sadface: Username is required"*. | Low |
| **TC-LGN-005** | **Logout Functionality** | User is logged in | 1. Click on the "Hamburger Menu" (top left).<br>2. Click "Logout" in the sidebar. | User is redirected back to the Login page. | Medium |

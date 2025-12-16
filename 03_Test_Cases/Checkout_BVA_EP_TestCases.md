# 🔢 Test Suite: Checkout Information Validation
**Module:** Checkout: Your Information  
**Techniques:** Equivalence Partitioning (EP), Boundary Value Analysis (BVA)  
**URL:** https://www.saucedemo.com/checkout-step-one.html

---

## 🧠 Test Data Strategy
To ensure the robustness of the "Postal Code" field, we apply standard validation rules (simulating a US 5-digit Zip Code requirement).

### 1. Equivalence Partitioning (EP)
We divide input data into classes:
* **Valid Class:** Numeric, exactly 5 digits.
* **Invalid Class:** Empty field.
* **Invalid Class:** Non-numeric characters (Special symbols, Letters).

### 2. Boundary Value Analysis (BVA)
Assumed Requirement: Zip Code must be exactly 5 digits.
* **Min Boundary (-1):** 4 digits (Invalid)
* **Target:** 5 digits (Valid)
* **Max Boundary (+1):** 6 digits (Invalid)

---

## 🧪 Test Cases

| TC ID | Title | Input Data (Zip/Postal) | Technique | Expected Result | Priority |
|---|---|---|---|---|---|
| **TC-CHK-001** | **Valid Zip Code** | `90210` (First Name: "John", Last Name: "Doe") | **EP (Valid)** | System accepts the input. User is redirected to "Checkout: Overview" page. | High |
| **TC-CHK-002** | **Empty Zip Code** | `[Empty]` | **EP (Invalid)** | Error message: *"Error: Postal Code is required"* | High |
| **TC-CHK-003** | **Boundary Min-1 (Too Short)** | `1234` (4 digits) | **BVA** | System should reject input or highlight field (Validation Error). | Medium |
| **TC-CHK-004** | **Boundary Max+1 (Too Long)** | `123456` (6 digits) | **BVA** | System should reject input or truncate to 5 digits. | Medium |
| **TC-CHK-005** | **Special Characters** | `12#$5` | **EP (Invalid)** | System should reject special characters. | Low |
| **TC-CHK-006** | **Letters in Zip Code** | `ABCDE` | **EP (Invalid)** | System should reject non-numeric characters. | Low |

> **Note for Reviewer:** Since SauceDemo is a test site, it has loose validation (it accepts "1" or "abc" as a Zip Code). In a real production environment, TC-CHK-003 through TC-CHK-006 would fail if validation logic were implemented correctly. These cases demonstrate the **design technique** rather than the site's current limitation.

# Bank Account App Assignment

## Overview
The task is to create a **Bank Account App** using Angular. The app should have five pages, each featuring tables, routing, and unique forms. The goal is to evaluate your understanding of Angular concepts, including components, routing, forms, and data binding.

---

## Pages Description

### 1. Dashboard Page
**Description:**  
A summary view displaying all the user's bank accounts with essential details. This page acts as the entry point after login.

**Key Features:**
- **Table:**
  - Columns:
    - Account Number
    - Account Type
    - Balance
    - Last Transaction Date
  - Actions:
    - Button to "View Account Details".
- **Routing:**
  - Clicking the "View Account Details" button routes to the **Account Details Page**.
- **Form:**
  - A search bar at the top to filter accounts by account number or type.

---

### 2. Account Details Page
**Description:**  
Displays detailed information about a specific account, including transaction history.

**Key Features:**
- **Table:**
  - Columns:
    - Transaction ID
    - Date
    - Description
    - Amount (Credit/Debit)
    - Balance After Transaction
  - Pagination for large transaction histories.
- **Routing:**
  - Linked from the Dashboard Page via the "View Account Details" button.
  - Back button to return to the Dashboard Page.
- **Form:**
  - A dropdown to filter transactions by date range (e.g., last week, last month).

---

### 3. Fund Transfer Page
**Description:**  
A page to transfer funds between the user's accounts or to other beneficiaries.

**Key Features:**
- **Table:**
  - Displays a list of recent transfers made by the user.
  - Columns:
    - Transaction ID
    - Beneficiary Name
    - Account Number
    - Transfer Amount
    - Date
    - Status
- **Routing:**
  - Standalone route `/fund-transfer`.
  - Success message routes back to the Dashboard or remains on the page.
- **Form:**
  - Inputs:
    - Sender Account (dropdown with user’s accounts).
    - Receiver Name.
    - Receiver Account Number.
    - Amount.
    - Remarks (optional).
  - Submit button to execute the transfer.

---

### 4. Account Creation Page
**Description:**  
A form to create a new bank account for the user.

**Key Features:**
- **Table:**
  - Displays existing accounts of the user.
  - Columns:
    - Account Number
    - Account Type
    - Creation Date
    - Status
- **Routing:**
  - Standalone route `/create-account`.
  - After successful account creation, routes back to the Dashboard.
- **Form:**
  - Inputs:
    - Account Type (dropdown: Savings, Current, Fixed Deposit).
    - Initial Deposit Amount.
    - Optional Account Nickname.
  - Submit button to create the account.

---

### 5. Profile Management Page
**Description:**  
A page to manage user profile information and update details.

**Key Features:**
- **Table:**
  - Displays existing user information in read-only format:
    - Name
    - Email
    - Phone Number
    - Address
- **Routing:**
  - Standalone route `/profile`.
  - Links for logout or updating specific sections route to relevant forms.
- **Form:**
  - Inputs to edit details:
    - Name
    - Email
    - Phone Number
    - Address
  - Update button to save changes.

---

## Requirements
1. Implement **Angular Routing** with dedicated route paths for each page.
2. Use **Angular Forms (Template-driven or Reactive)** for all input handling.
3. Integrate tables for data display with proper styling and pagination (where applicable).
4. Ensure a consistent design and layout using CSS or libraries like Angular Material.
5. Demonstrate state management where applicable (e.g., passing account data to the Account Details Page).

---

## Submission Guidelines
- Share your project repository link (GitHub, GitLab, etc.) with a clear README explaining how to run the app.
- Ensure the app is fully functional and meets the described requirements.
- Use proper coding standards and comments to explain your logic.

Good luck!

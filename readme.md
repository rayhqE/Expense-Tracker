# Expense Tracker

A simple Expense Tracker built using **HTML, CSS, and JavaScript**.  
It allows users to add, delete, and track expenses, with data saved using **Local Storage** so it stays even after refreshing the page.

---

## JavaScript Logic (Simple & Short)

### 1️⃣ DOM Content Loaded

- JavaScript runs only after the page loads using `DOMContentLoaded`.
- All form inputs, list, and total display elements are selected using `getElementById`.

---

### 2️⃣ Loading Saved Expenses

- Expenses are fetched from `localStorage` using `JSON.parse`.
- If no data exists, an empty array is used.
- Expenses are rendered and total amount is calculated on page load.

---

### 3️⃣ Adding a New Expense

- On form submit:
  - Default reload is prevented using `preventDefault()`.
  - Expense name and amount are validated.
  - A new expense object is created with a unique `id` using `Date.now()`.
  - Expense is saved to the array and local storage.

---

### 4️⃣ Rendering Expenses

- The expense list is cleared and re-rendered every time data changes.
- Each expense is displayed with a **Delete** button.
- Uses `innerHTML` to dynamically update the list.

---

### 5️⃣ Calculating & Updating Total

- Total amount is calculated using `reduce()`.
- The total is updated whenever an expense is added or deleted.
- Displayed with two decimal places using `toFixed(2)`.

---

### 6️⃣ Deleting an Expense

- Uses event delegation on the expense list.
- When a delete button is clicked:
  - Expense ID is retrieved.
  - That expense is removed using `filter()`.
  - Updated data is saved and UI refreshed.

---

## Features

- Add and delete expenses
- Persistent data using Local Storage
- Automatic total calculation
- Clean and simple logic
- Uses modern JavaScript methods

---

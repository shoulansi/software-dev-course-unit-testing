## 🛒 Shopping Cart Unit Testing Activity

### 🎯 Objective:
Students will practice writing unit tests to verify the behavior of a shopping cart program's methods. This activity reinforces the concepts of creating meaningful test cases, including positive, negative, and edge cases, and using assertions to validate behavior.

---

### 📋 Instructions:

---

#### 🔧 Setup

1. **Create a project folder** named `shopping-cart`.

2. **Initialize the project:**
```bash
npm init -y
```

### 📦 Install Jest:

Use the following command to install Jest as a development dependency:

```bash
npm install --save-dev jest
```

### 🛠️ Add a Test Script to `package.json`:

Update the `scripts` section in your `package.json` file to include a test command for Jest:

```json
"scripts": {
  "test": "jest"
}
```

## 🧩 Task

Implement and test a basic shopping cart module. The module should include the following methods:

- `addItem(cart, item, quantity)`: Adds an item to the cart.
- `removeItem(cart, item)`: Removes an item from the cart.
- `getTotalItems(cart)`: Returns the total number of items in the cart.

---

## 🛠️ Steps

### 1️⃣ Define the Module:
- Create a file named `cart.js`.
- Define the required methods.
- Export the methods using `module.exports`.

---

### 2️⃣ Write Unit Tests:
- Create a `tests` folder.
- Inside, add a file named `cart.test.js`.
- Write tests for each method in the `cart.js` module, covering:

  - ✅ **Positive Tests**: Valid inputs producing expected results.
  - ❌ **Negative Tests**: Invalid inputs handled gracefully.
  - ⚠️ **Edge Cases**: Unusual or extreme values.

---

### 3️⃣ Run the Tests:

```bash
npm test
```

Execute the tests and verify that all pass.

---

### 4️⃣ Refactor:
If any tests fail, modify the implementation in `cart.js` until all tests pass.

---

## 📊 Example Scenarios for Testing:

### 🔹 addItem:

- **Positive**: Add a new item with a valid name and quantity.
- **Negative**: Add an item with a negative quantity.
- **Edge Case**: Add an item with a quantity of 0.

---

### 🔹 removeItem:

- **Positive**: Remove an existing item from the cart.
- **Negative**: Attempt to remove an item not in the cart.
- **Edge Case**: Remove the last item from the cart.

---

### 🔹 getTotalItems:

- **Positive**: Calculate the total number of items correctly.
- **Negative**: Handle an empty cart.
- **Edge Case**: Calculate with large quantities.

---

✅ Complete the task by ensuring your test suite is robust and demonstrates an understanding of unit testing best practices.

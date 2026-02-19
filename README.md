# User Profile Manager - Data Types Deep Dive 🚀

A simple JavaScript project demonstrating the fundamental differences between **Primitive** and **Reference** data types. This project explores memory management, immutability, and the behavior of Stack vs. Heap.

## 📌 Project Overview
This project was built to visualize how JavaScript handles data storage:
- **Primitive Types:** Stored by **Value** in the Stack.
- **Reference Types:** Stored by **Reference** (Memory Address) in the Heap.

## 🧠 Key Concepts Learned

### 1. Primitive Data Types
*   **Behavior:** Copy by Value.
*   **Immutability:** Once created, the value cannot be changed; a new value is assigned instead.
*   **Example:** Strings, Numbers, Booleans.
*   **Observation:** Changing the copied variable does **not** affect the original variable.

### 2. Reference Data Types
*   **Behavior:** Copy by Reference.
*   **Mutability:** Properties can be modified because multiple variables point to the same memory location.
*   **Example:** Objects, Arrays.
*   **Observation:** Changing a property through one reference **affects all** variables pointing to that object.

## 💻 Code Example

```javascript
// Primitive Example
let myName = "Guna";
let friendName = myName; 
friendName = "Surya"; 
console.log(myName); // Output: "Guna" (Remains unchanged)

// Reference Example
let myHouse = { color: "blue" };
let friendKey = myHouse; 
friendKey.color = "white"; 
console.log(myHouse.color); // Output: "white" (Changed!)
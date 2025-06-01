````markdown
# Chunky Monkey Algorithm

This project implements the **Chunky Monkey Algorithm** in JavaScript. The goal is to split an array into groups (or "chunks") of a specified length and return them as a two-dimensional array.

## 🧠 User Stories

- ✅ Write a function named `chunkArrayInGroups`.
- ✅ The function takes two parameters:
  - `arr` (Array): the array to split
  - `size` (Number): the number of elements per chunk
- ✅ The function splits the array into sub-arrays of the given size.
- ✅ The function returns a two-dimensional array containing these chunks.

## 📦 Example Usage

```javascript
function chunkArrayInGroups(arr, size) {
  let result = [];

  for (let i = 0; i < arr.length; i += size) {
    result.push(arr.slice(i, i + size));
  }

  return result;
}

// Example 1
console.log(chunkArrayInGroups(["a", "b", "c", "d"], 2));
// Output: [["a", "b"], ["c", "d"]]

// Example 2
console.log(chunkArrayInGroups([0, 1, 2, 3, 4, 5], 4));
// Output: [[0, 1, 2, 3], [4, 5]]
```

## 📁 Project Structure

```
chunky-monkey/
├── index.js       # Core algorithm implementation
└── README.md      # Project documentation
```

## ✅ Tests to Pass

The function should return correct outputs for:

* Chunk sizes that evenly divide the array.
* Chunk sizes that don’t evenly divide the array.
* Empty arrays or zero-size chunks (optional edge case handling).

## 🛠 Technologies Used

* JavaScript (ES6+)
* Node.js (for running scripts in the terminal, optional)

## 🚀 Getting Started

You can copy the `chunkArrayInGroups` function into your own JavaScript environment or Node.js setup. Run it with:

```bash
node index.js
```

## 📬 License

This project is open-source and free to use for educational purposes.

```

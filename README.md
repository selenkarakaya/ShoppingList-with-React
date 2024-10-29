# Shopping List 📋

## Overview
- I have started to learn React, and this project is a demonstration of my learning process. It includes components and uses core React hooks like `useState` and `useEffect`. The **Shopping List** app allows users to add, edit, and delete items, providing a simple and interactive experience for managing a shopping list.

### Features
- **Add Items**: Quickly add new items to the shopping list.
- **Edit Items**: Modify existing items in the list.
- **Delete Items**: Remove items from the list when no longer needed.
- **React Hooks**: Utilizes React hooks like `useState` for managing state.
- **Local State Management**: Keeps everything managed locally for fast performance.

## Technologies Used
- React: For building the user interface.
- JavaScript (ES6+): Core language for building components and managing logic.
- HTML/CSS: For structuring and styling the app.
- Node.js & npm: For managing dependencies and running the development environment.

## Usage
- **Add Item**: Use the input field to type an item name and click the "Add" button. The item will appear in the shopping list.
- **Edit Item**: Click the "Edit" button next to any item to modify its name. After editing, press "Save" to update the item.
- **Delete Item**: Click the "Delete" button next to an item to remove it from the list.

## Demo 🔗
You can check out a live demo of the Shopping List ([https://grocerychecklist.netlify.app/]).

## Installation
To run the **Shopping List** app on your local machine:

### Prerequisites

- You need to have **Node.js** installed on your computer.

### Steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/ShoppingList-with-React.git
   ```

2. Navigate to the project directory:
   ```bash
   cd ShoppingList-with-React
   ```

3. Install dependencies:
   ```bash
   npm install
   ```

4. Start the development server:
   ```bash
   npm start
   ```

5. Open your browser and visit:
   ```
   http://localhost:3000
   ```

You should now be able to see and interact with your Shopping List app!

### Example:

```javascript
const [items, setItems] = useState([]);

// Add new item
const addItem = (newItem) => {
  setItems([...items, newItem]);
};

// Edit an item
const editItem = (id, updatedItem) => {
  const updatedItems = items.map((item) =>
    item.id === id ? updatedItem : item
  );
  setItems(updatedItems);
};

// Delete an item
const deleteItem = (id) => {
  const updatedItems = items.filter((item) => item.id !== id);
  setItems(updatedItems);
};
```

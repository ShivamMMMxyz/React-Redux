# React Redux Counter App

A simple **Increment/Decrement counter** built using **React** and **Redux**.  
This project demonstrates the basics of Redux state management in a React application.

---

## 🚀 Features
- Increment and decrement a counter
- State management using Redux
- Clean and minimal UI

---

## 📂 Project Structure
redux-counter-app/
├── public/
│ └── index.html # Main HTML file
│
├── src/
│ ├── actions/
│ │ └── index.js # Action creators (incNumber, decNumber)
│ │
│ ├── reducers/
│ │ ├── index.js # Root reducer (combineReducers)
│ │ └── upDown.js # Counter reducer (increment/decrement logic)
│ │
│ ├── store.js # Redux store configuration
│ │
│ ├── App.js # Main component with UI + dispatching actions
│ ├── App.css # Styles for UI
│ ├── index.js # Entry point, wraps App with Provider
│ │
│ └── ... (other CRA/Vite boilerplate files)
│
├── package.json # Dependencies and scripts
└── README.md # Project documentation

---

## 📜 File Details

- **`src/actions/index.js`**  
  Defines action creators:
  - `incNumber()` → Increment action  
  - `decNumber()` → Decrement action  

- **`src/reducers/upDown.js`**  
  Reducer function to handle increment/decrement logic.

- **`src/reducers/index.js`**  
  Combines reducers using `combineReducers`.

- **`src/store.js`**  
  Configures and exports the Redux store.

- **`src/App.js`**  
  Main React component.  
  - Displays counter UI.  
  - Uses `useSelector` to read state.  
  - Uses `useDispatch` to trigger increment/decrement actions.  

- **`src/App.css`**  
  Contains styling for the UI (counter box, buttons, etc.).

- **`src/index.js`**  
  Entry point of the app. Wraps `<App />` inside `<Provider store={store}>`.

---
# React.js: What It Is, Its Advantages, and How to Install It

<img src="https://upload.wikimedia.org/wikipedia/commons/a/a7/React-icon.svg" width="100" height="100" />

### A simple beginner-friendly guide to understanding React.js and setting up your first React project

If you are learning web development, you have probably heard the name **React.js** many times.

I started learning React after getting familiar with HTML, CSS, and JavaScript. At first, React looked a little confusing because there were new concepts like components, JSX, props, and state.

But once I understood the basic idea behind React, it became much easier.

So in this article, I want to explain React.js in a simple way — what it is, why developers use it, its advantages, and how you can install it and create your first React project.

---

## What is React.js?

React.js is a **JavaScript library used to build user interfaces**, especially for web applications.

It was originally developed by Facebook and is now maintained as an open-source project.

The main idea behind React is to build a website using **small, reusable components**.

### Component-Based Architecture

```
┌─────────────────────────────────┐
│      E-commerce Website          │
├─────────────────────────────────┤
│            Navbar               │
├─────────────────────────────────┤
│  ┌──────────┐  ┌──────────┐    │
│  │ Product  │  │ Product  │    │
│  │  Card    │  │  Card    │    │
│  └──────────┘  └──────────┘    │
├─────────────────────────────────┤
│        Product List              │
├─────────────────────────────────┤
│        Login Form                │
├─────────────────────────────────┤
│          Footer                  │
└─────────────────────────────────┘
```

For example, imagine you are creating an e-commerce website.

Instead of writing everything in one huge file, you can create separate components such as:

-  **Navbar** - Navigation menu
-  **Product Card** - Individual product display
-  **Product List** - Grid of products
-  **Login Form** - User authentication
-  **Footer** - Footer section
-  **Button** - Reusable button component

You can then reuse these components wherever you need them.

✨ **This makes the application easier to develop, understand, and maintain.**

---

## React.js is a Library, Not a Programming Language

One common mistake beginners make is calling React a programming language.

React.js is **not a programming language**.

It is a **JavaScript library**.

JavaScript is the programming language, while React provides tools and concepts that help us build user interfaces more efficiently.

So, if you want to learn React, having a good understanding of JavaScript is very helpful.

---

## Why Do Developers Use React.js?

When a website becomes bigger, managing every part of the interface using only HTML, CSS, and JavaScript can become difficult.

React helps organize the interface into smaller parts.

For example:

```jsx
function Welcome() {
  return <h1>Welcome to my website!</h1>;
}
```
## How to Install React.js

<img src="https://img.icons8.com/color/96/000000/npm.png" width="100" height="100" />

Now that we understand what React.js is and how we use it, let's see how to set up React on our computer.

For creating a new React project, we can use **Vite**. It provides a simple and fast way to set up a React application.

**Before starting, make sure you have Node.js installed on your computer.**

### Prerequisites:
- ✅ Node.js (v14 or higher)
- ✅ npm (comes with Node.js)
- ✅ Visual Studio Code
- ✅ Basic JavaScript knowledge

---

### Step 1: Install Node.js

First, download and install Node.js on your computer.

After installing it, open **Command Prompt** or the **VS Code Terminal** and check whether Node.js is installed correctly.

Run:

```bash
node -v
```
If both commands show a version number, Node.js and npm are installed successfully.

---

### Step 2: Open VS Code

Open **Visual Studio Code** and create or select the folder where you want to create your React project.

Then open the terminal:

**Terminal → New Terminal**

---

### Step 3: Create a React Project

In the VS Code terminal, run the following command:

```bash
npm create vite@latest
```
Vite will ask you some questions.

#### Project Name

Enter the name of your project:

```text
Project name: my-react-app
```

You can use any name you want.

#### Select a Framework

Choose:

```text
React
```

#### Select a Variant

Choose:

```text
JavaScript
```

After selecting these options, Vite will create your React project.

---

### Step 4: Open the Project Folder

Now move into your newly created project folder:

```bash
cd my-react-app
```

Replace `my-react-app` with your project name if you selected a different name.

---

### Step 5: Install Dependencies

Now we need to install the packages required by our React project.

Run:

```bash
npm install
```

This may take a few seconds or minutes depending on your internet connection.

Once the installation is complete, your project is ready to run.

---

### Step 6: Start the React Application

Now run the following command:

```bash
npm run dev
```

You will see a local address in the terminal, something like:

```text
Local: http://localhost:5173/
```

Open this address in your browser.

You should now see your React application running.

 **Congratulations! Your first React project is ready.**

---

# How to Use React After Installation

Once the React project is created, open it in VS Code.

### Project File Structure

You will find a `src` folder containing files such as:

```
my-react-app/
├── src/
│   ├── App.jsx          ← Main component
│   ├── App.css          ← Styles for App
│   ├── main.jsx         ← Entry point
│   └── index.css        ← Global styles
├── index.html              ← HTML file
├── package.json            ← Dependencies
└── vite.config.js          ← Vite config
```

The main file we will work with as a beginner is:

**`App.jsx`** - This is where you write your React components

Open `App.jsx` and replace the existing code with:

```jsx
function App() {
  return (
    <div>
      <h1>Hello, React!</h1>
      <p>This is my first React application.</p>
    </div>
  );
}

export default App;
```

Save the file and check your browser.

You will see:

**Hello, React!**

This is a simple example of how we start using React to create a user interface.

---

# Basic React Workflow

### Visual Workflow Diagram

```
┌──────────────────────────────────────────────────────┐
│              React Development Workflow               │
└──────────────────────────────────────────────────────┘

  1️⃣  Install Node.js
         ↓
  2️⃣  Create React Project (using Vite)
         ↓
  3️⃣  Install Dependencies (npm install)
         ↓
  4️⃣  Start Development Server (npm run dev)
         ↓
  5️⃣  Write React Components (JSX code)
         ↓
  6️⃣  Hot Reload in Browser (automatic)
         ↓
  7️⃣  Build for Production (npm run build)
```

### Key React Concepts to Learn Next:

| Concept | Description |
|---------|-------------|
| 🧩 **JSX** | JavaScript XML - write HTML in JavaScript |
| 🔧 **Components** | Reusable UI building blocks |
| 📦 **Props** | Pass data between components |
| 💾 **State** | Store and manage component data |
| 🪝 **Hooks** | Functions like useState, useEffect |
| 🎯 **Events** | Handle user interactions |
| 📝 **Forms** | Create and validate forms |
| 🌐 **API Integration** | Fetch data from servers |

---

## Next Steps 

Once you understand this basic process, you'll be ready to:

✨ Build interactive user interfaces

✨ Create reusable component libraries

✨ Manage application state effectively

✨ Connect to real APIs and databases

**Happy coding with React!** 💚

---

## About the Author

**Written by:** _Aishwarya Koche_

**Date:** September 2, 2026

*This guide was created to help beginners understand React.js and get started with their first React project.*
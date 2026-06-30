# React + TypeScript + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Oxc](https://oxc.rs)
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/)

## React Compiler

The React Compiler is not enabled on this template because of its impact on dev & build performances. To add it, see [this documentation](https://react.dev/learn/react-compiler/installation).

## Expanding the ESLint configuration

If you are developing a production application, we recommend updating the configuration to enable type-aware lint rules:

```js
export default defineConfig([
  globalIgnores(['dist']),
  {
    files: ['**/*.{ts,tsx}'],
    extends: [
      // Other configs...

      // Remove tseslint.configs.recommended and replace with this
      tseslint.configs.recommendedTypeChecked,
      // Alternatively, use this for stricter rules
      tseslint.configs.strictTypeChecked,
      // Optionally, add this for stylistic rules
      tseslint.configs.stylisticTypeChecked,

      // Other configs...
    ],
    languageOptions: {
      parserOptions: {
        project: ['./tsconfig.node.json', './tsconfig.app.json'],
        tsconfigRootDir: import.meta.dirname,
      },
      // other options...
    },
  },
])
```

You can also install [eslint-plugin-react-x](https://github.com/Rel1cx/eslint-react/tree/main/packages/plugins/eslint-plugin-react-x) and [eslint-plugin-react-dom](https://github.com/Rel1cx/eslint-react/tree/main/packages/plugins/eslint-plugin-react-dom) for React-specific lint rules:

```js
// eslint.config.js
import reactX from 'eslint-plugin-react-x'
import reactDom from 'eslint-plugin-react-dom'

export default defineConfig([
  globalIgnores(['dist']),
  {
    files: ['**/*.{ts,tsx}'],
    extends: [
      // Other configs...
      // Enable lint rules for React
      reactX.configs['recommended-typescript'],
      // Enable lint rules for React DOM
      reactDom.configs.recommended,
    ],
    languageOptions: {
      parserOptions: {
        project: ['./tsconfig.node.json', './tsconfig.app.json'],
        tsconfigRootDir: import.meta.dirname,
      },
      // other options...
    },
  },
])
```
# 📚 Student CRUD Application

A simple and responsive **Student CRUD (Create, Read, Update, Delete) Application** built using **React, TypeScript, and Vite**. This project demonstrates the implementation of CRUD operations with a clean component structure and local data persistence.

---

## 🚀 Project Overview

The Student CRUD Application allows users to manage student records efficiently. Users can:

* ➕ Add new students
* 📖 View all student records
* ✏️ Edit existing student details
* 🗑️ Delete student records

The project is designed to help beginners understand how CRUD operations work in modern React applications while following a modular folder structure.

---

# ✨ Features

* Create student records
* Read and display all students
* Update student information
* Delete student records
* Built with React Functional Components
* TypeScript support
* Organized API folder structure
* Responsive and lightweight
* Fast development using Vite

---

# 🛠️ Tech Stack

### Frontend

* React 19
* TypeScript
* Vite
* CSS

---

# 📂 Project Structure

```text
crud-app/
│
├── src/
│   ├── api/
│   │   ├── CREATE/
│   │   ├── READ/
│   │   ├── UPDATE/
│   │   └── DELETE/
│   │
│   ├── assets/
│   ├── type/
│   ├── App.tsx
│   ├── App.css
│   ├── main.tsx
│   └── index.css
│
├── public/
├── package.json
├── vite.config.ts
└── README.md
```

---

# ⚙️ Installation

Clone the repository

```bash
git clone https://github.com/your-username/your-repository-name.git
```

Move into the project directory

```bash
cd crud-app
```

Install dependencies

```bash
npm install
```

Run the development server

```bash
npm run dev
```

Open your browser

```
http://localhost:5173
```

---

# 🧩 CRUD Operations

## ➕ Create

* Enter student name.
* Enter student email.
* Click **Add**.
* A new student record is created.

---

## 📖 Read

* Displays all available student records.
* Shows student name and email.

---

## ✏️ Update

* Click the **Edit** button.
* Modify the student information.
* Click **Update** to save the changes.

---

## 🗑️ Delete

* Click the **Delete** button.
* The selected student record is removed instantly.

---

# 📸 Application Flow

```
Enter Student Details
        │
        ▼
Click Add Button
        │
        ▼
Student List Updates
        │
        ▼
Edit or Delete Records
        │
        ▼
Updated Student List
```

---

# 📚 Learning Outcomes

This project helped in understanding:

* React Hooks (`useState`)
* Component-based architecture
* TypeScript interfaces
* CRUD logic implementation
* State management
* Event handling
* Folder organization
* Modular code structure
* Building projects using Vite

---

# 💡 Future Improvements

Some features that can be added in future versions:

* Backend integration (Node.js / Express)
* MongoDB database
* User authentication
* Search functionality
* Filter students
* Pagination
* Form validation
* Toast notifications
* Dark Mode
* Responsive dashboard UI
* REST API integration

---

# 🎯 Use Case

This project is suitable for:

* React beginners
* TypeScript learners
* College mini projects
* CRUD operation practice
* Frontend development portfolio
* Interview preparation

---

# 📦 Available Scripts

Run development server

```bash
npm run dev
```

Build production version

```bash
npm run build
```

Preview production build

```bash
npm run preview
```

Lint the project

```bash
npm run lint
```

---

# 🤝 Contributing

Contributions are welcome.

1. Fork the repository.
2. Create a new feature branch.
3. Commit your changes.
4. Push the branch.
5. Open a Pull Request.

---

# ⭐ Support

If you found this project useful, consider giving it a ⭐ on GitHub. It helps others discover the project and motivates further improvements.

---

# 👨‍💻 Author

**Prakhar Porwal**

Frontend Developer | React Developer | Aspiring AI/ML Engineer

If you like this project, feel free to connect and explore my other repositories.

---

## 📄 License

This project is created for educational and learning purposes. You are free to use, modify, and improve it for personal or academic projects.


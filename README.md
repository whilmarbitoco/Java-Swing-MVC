# 🎨 Swing MVC Template 🎉

This project is a **Swing MVC Template** designed to help developers structure their Java applications using the **Model-View-Controller (MVC)** design pattern. The template offers a modular and reusable structure for managing user interactions, data, and UI components effectively. 🚀 This template serves as the foundation for my other project, [NoSnitch](https://github.com/whilmarbitoco/NoSnitch). 🌟

---

## 📂 Project Structure 📁

```
src
├── controllers          # 🎮 Application controllers
│   ├── Controller.java          # 🧩 Base controller class
│   ├── LoginController.java     # 🔑 Handles login logic
│   └── SignupController.java    # 📝 Handles signup logic
├── core                 # 🛠️ Core utilities for the application
│   ├── Auth.java                # 🛡️ Handles authentication operations
│   └── Prompt.java              # 💬 Displays user prompts and alerts
├── models               # 🗂️ Application data models
│   ├── data                    # 🗃️ Serialized data for persistence
│   │   ├── Comment.ser          # 💬 Stores comment data
│   │   ├── Post.ser             # 📝 Stores post data
│   │   ├── Session.ser          # 🔑 Stores session data
│   │   └── User.ser             # 👤 Stores user data
│   ├── Model.java               # 🧩 Base model class with serialization
│   ├── Models.java              # 📊 Provides a registry for all models
│   ├── Session.java             # 🕒 Represents user session data
│   └── User.java                # 👤 Represents a user entity
├── nosnitch              # 🏁 Main application entry point
│   └── NoSnitch.java           # 🚀 Application launcher
└── views                # 🎨 User interface components
    ├── LoginView.form           # 🔑 GUI layout for login view
    ├── LoginView.java           # 🔧 Logic for login view
    ├── SignUpView.form          # 📝 GUI layout for signup view
    └── SignUpView.java          # 🔧 Logic for signup view
```

---

## 🧩 Core Components 🔍

### **Base Controller (Controller.java)**
The `Controller` class serves as a foundation for all controllers. It connects views to the core logic and models while managing user actions and transitions. ✨  
- **`exit`:** Allows the user to exit the application gracefully, with options for session handling.  
- **`logout`:** Handles user logout and session cleanup.

### **Base Model (Model.java)**  
The `Model` class is a generic, serializable foundation for all data models. It provides built-in support for:  
- **CRUD operations**: Add, update, and retrieve data.
- **Serialization**: Automatically saves and loads data to `.ser` files for persistence.  
- **Cleanup logic**: Removes outdated entries based on time conditions.  
- **Dynamic ID generation**: Ensures unique identifiers for stored data.

---

## 🚀 Usage 🛠️

1. **Clone the Repository**  
   ```bash
   git clone https://github.com/whilmarbitoco/Java-Swing-MVC.git
   ```

2. **Open in NetBeans** 🖥️  
   Open the project in **NetBeans IDE**, as the `.form` files are designed for seamless integration with it.

3. **Run the Application** 🎉  
   Launch the application by running the `NoSnitch.java` file. 🏁

4. **Extend Functionality** 🔍  
   - Create new controllers to handle additional business logic.  
   - Add or modify models to represent new data entities.  
   - Use NetBeans GUI builder to add new `.form` and `.java` files for views.

---

## 🌟 Features ✨

- **📦 Modular Structure:** Separation of concerns between models, views, and controllers.  
- **💾 Persistence:** Automatically saves and loads data using serialized files (`.ser`).  
- **🔐 Authentication:** Built-in authentication and session management.  
- **🎨 Swing Integration:** Designed for GUI creation with NetBeans.  
- **🕒 Cleanup Functionality:** Built-in support for maintaining clean datasets over time.

---

## 🌈 How to Customize

- **Add Views:** 🖌️ Create `.form` and `.java` files in the `views` directory.  
- **Add Controllers:** 🕹️ Extend the `Controller` class for new functionalities.  
- **Define Models:** 🗂️ Extend the `Model` class for new entities.  
- **Extend Core Utilities:** Add helpers in the `core` package for reusable logic.  

---

## 📜 License 📝

This project is licensed under [MIT License](LICENSE).  

---

### © 2024 Whilmar Bitoco 👨‍💻
All rights reserved. This project and its code are authored by **Whilmar Bitoco**. ✨


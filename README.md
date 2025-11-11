## 📄 README: Pg-Server-ClassWork 

This project is a **Node.js/Express.js REST API** for managing **Users**, utilizing **PostgreSQL** as the database backend.

---

### ✨ Key Features

* **CRUD** operations for the **User** entity.
* **PostgreSQL** for data storage (using the `pg` library).
* Input data **validation** for user creation (`yup`).
* **Pagination** support for the user list.
* Centralized **error handling**.
* The `User` model is implemented as a **class** for database interaction.

---

### ⚙️ Technologies

| Category | Technology |
| :--- | :--- |
| **Server** | Node.js, Express.js |
| **Database** | PostgreSQL, `pg` |
| **Validation** | `yup` |
| **Utilities** | `http-errors`, `query-parser-express` |

---

### 🚀 API Endpoints

Base URL: `http://localhost:5000`

| Method | Endpoint | Action |
| :---: | :--- | :--- |
| **POST** | `/users` | Create a user (with validation) |
| **GET** | `/users` | Retrieve list (supports pagination: `?page=1&results=10`) |
| **GET** | `/users/:userId` | Get user by ID |
| **PATCH** | `/users/:userId` | Update user by ID |
| **DELETE** | `/users/:userId` | Delete user by ID |

---

### 🛠️ Setup and Running

1.  **Cloning and Installation:**
    ```bash
    git clone [repository-link]
    cd Pg-Server-ClassWork
    npm install
    ```
2.  **PostgreSQL Configuration:**
    * Create your database and a `users` table.
    * **Update** the PostgreSQL connection parameters (`user`, `password`, `database`, etc.) in the `models/index.js` file.
3.  **Running the Server:**

    Use the following commands, based on your `package.json` scripts:

    * **Development Mode** (with automatic restart on changes):
        ```bash
        npm run dev
        ```
    * **Production/Standard Mode** (single run):
        ```bash
        npm start
        ```

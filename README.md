# Flask Gaming App

Welcome to the Flask Gaming App! This is a web application built with Flask that allows users to browse gaming products, manage their cart, and interact with an admin dashboard for product and customer management. The app is designed for both users and administrators, with separate functionalities for each role.

---

## Live Link: https://my-flask-gaming-app.onrender.com

## Features

### Currently Working Features

1. **User and Admin Authentication**:
   - Users and admins can sign up and log in.
   - Admins have access to a dedicated dashboard for managing products and customers.

2. **Admin CRUD Operations**:
   - Admins can create, read, update, and delete (CRUD) products and customer details.

3. **User Cart Management**:
   - Users can view products, add items to their cart, and delete items from their cart.

4. **Search Functionality**:
   - Users can search for products using the search bar.

5. **Stock Management**:
   - Admins can manage product stock levels through the admin dashboard.

---

### Features to be Added in the Future

1. **Order Placement**:
   - Users will be able to place orders (currently incomplete).

2. **PC Builder Feature**:
   - A feature to allow users to build and customize their PCs.

3. **Product Categories**:
   - Products will be organized into categories for easier navigation.

4. **M-Pesa API Integration**:
   - Payment integration using the M-Pesa API is currently not implemented and will be added in the future.

---

## Technologies Used

- **Backend**: Flask (Python)
- **Frontend**: HTML, CSS, JavaScript, Jinja2 Templating
- **Database**: SQLAlchemy (SQLite/PostgreSQL)
- **Authentication**: Flask-Login
- **Password Hashing**: Werkzeug Security
- **Environment Management**: `python-dotenv`
- **Form Handling**: Flask-WTF
- **Error Handling**: Custom 404 Error Page

---

## Technical Features

1. **Modular Code Structure**:
   - The app is structured using Flask Blueprints for better organization and scalability.
   - Blueprints are used for `views`, `auth`, and `admin` functionalities.

2. **Secure Authentication**:
   - User passwords are hashed using Werkzeug's `generate_password_hash` and verified using `check_password_hash`.
   - Flask-Login manages user sessions and authentication.

3. **Database Models**:
   - SQLAlchemy is used to define and manage database models (`Customer`, `Product`, `Cart`, `Order`).
   - Relationships between models (e.g., `Customer` to `Cart`, `Product` to `Order`) are implemented using SQLAlchemy's ORM.

4. **Error Handling**:
   - Custom 404 error page for better user experience.

5. **Environment Variables**:
   - Sensitive configuration (e.g., `SECRET_KEY`, `DATABASE_URL`) is managed using environment variables loaded from a `.env` file.

6. **Admin Dashboard**:
   - Admins can perform CRUD operations on products and customers through a dedicated dashboard.

7. **Cart Management**:
   - Users can add/remove items from their cart, with cart data linked to their account.

---

## How to Navigate the App

### Logging In as a User or Admin

1. Navigate to the top-right corner of the navbar.
2. Click on the **Account** dropdown.
3. Click on the **Login** button.
4. Enter your credentials to log in.

### Logging In as an Admin

- Use the pre-created admin account:
  - **Email**: `admin@gmail.com`
  - **Password**: `012345`

Once logged in as an admin, you will see a new entry for **Admin Dashboard** in the account dropdown on the navbar. This dashboard allows you to manage products and customers.

---

## Installation and Setup

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/bravvjr/my_flask_gaming_app.git
   cd my_flask_gaming_app
   ```

2. **Set Up a Virtual Environment**:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```

3. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Set Up the Database**:
   - Run the following commands to initialize the database:
     ```bash
     flask db init
     flask db migrate
     flask db upgrade
     ```

5. **Run the Application**:
   ```bash
   flask run
   ```
   - The app will be available at `http://127.0.0.1:5000/`.

---

## Contributing

Contributions are welcome! If you'd like to contribute to this project, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bugfix.
3. Commit your changes.
4. Push your branch and submit a pull request.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Contact

If you have any questions or suggestions, feel free to reach out:

-**Bravin Murambi
- **GitHub**: [bravvjr](https://github.com/bravvjr)
- **Email**: [bravvjr@gmail.com]

---

Thank you for checking out the Flask Gaming App! I hope you enjoy using it. 🚀

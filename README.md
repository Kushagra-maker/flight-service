# SkyRoute

## 📖 Overview
SkyRoute is a Node.js-based API designed to manage various aspects of flight operations, including airports, cities, airplanes, and seats. The project follows best coding practices and project management recommendations to ensure scalability and maintainability.

## 🛠️ Features
- **Flight Management**: CRUD operations for flights, including scheduling and allocation.
- **Airport and City Management**: Manage airports and cities to support flight operations.
- **Airplane and Seat Management**: Handle airplane details and seat configurations.
- **Search Functionality**: Filter flights based on parameters like price, departure, and arrival airports.
- **Microservices Architecture**: Designed for reliability and scalability.

## 📂 Project Structure
```
Flights-Service/
│── src/
│   ├── config/          # Configuration settings for libraries and modules
│   ├── routes/          # API route definitions
│   ├── middlewares/     # Request interceptors (validators, authenticators, etc.)
│   ├── controllers/     # Handle requests and interact with the business layer
│   ├── repositories/    # Handle database queries (ORM or raw SQL)
│   ├── services/        # Business logic layer
│   ├── utils/           # Helper functions, error classes, etc.
│── migrations/          # Sequelize migrations (created after initialization)
│── seeders/             # Sequelize seeders (created after initialization)
│── .env                 # Environment variables
│── package.json         # Project dependencies and scripts
│── README.md            # Documentation
```

## 🚀 Getting Started

### Prerequisites
- Install [Node.js](https://nodejs.org/)
- Install [npm](https://www.npmjs.com/)
- A relational database (e.g., MySQL, PostgreSQL, MariaDB)

### Installation Steps

1. **Clone the repository:**
   ```sh
   git clone https://github.com/swraj28/Flights-Service.git
   cd Flights-Service
   ```

2. **Install dependencies:**
   ```sh
   npm install
   ```

3. **Set up environment variables:**
   - Create a `.env` file in the root directory.
   - Add the following variables:
     ```env
     PORT=3000
     DB_USERNAME=<your_db_username>
     DB_PASSWORD=<your_db_password>
     DB_NAME=<your_db_name>
     DB_HOST=127.0.0.1
     DB_DIALECT=mysql
     ```
     Replace `<your_db_username>`, `<your_db_password>`, and `<your_db_name>` with your database credentials.

4. **Initialize Sequelize (for database migrations):**
   ```sh
   npx sequelize init
   ```
   This will generate `migrations/`, `seeders/`, and `config/config.json` inside the `src/config/` folder.

5. **Configure database settings:**
   - Open `src/config/config.json`.
   - Update the `development`, `test`, and `production` sections with your database credentials.

6. **Run database migrations:**
   ```sh
   npx sequelize db:migrate
   ```

7. **Run seeders (optional):**
   ```sh
   npx sequelize db:seed:all
   ```

8. **Start the development server:**
   ```sh
   npm run dev
   ```

## 🧪 Running Tests
To run tests, execute:
```sh
npm test
```

## 🤝 Contributing
We welcome contributions! If you have suggestions for improving this project, feel free to fork the repository, create a new branch, and submit a pull request.

## 📜 License
This project is licensed under the [MIT License](LICENSE).

---




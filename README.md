# ShipTrack Pro 🚚

**ShipTrack Pro** is a full-stack logistics and shipment management application designed to manage shipments, track delivery progress, and provide role-based access to logistics operations.

The project combines a React-based frontend, a Spring Boot REST API, and a PostgreSQL database to support shipment workflows and tracking operations.

## ✨ Features

- **Authentication and Authorization:** JWT-based authentication and role-based access control.
- **Shipment Management:** Create and manage shipment records.
- **Shipment Tracking:** Track shipment status and view tracking history.
- **Dashboard:** Access shipment information and operational metrics.
- **Address Management:** Manage shipment origin and destination addresses.
- **User and Role Management:** Organize access for customers, business clients, logistics operators, and administrators.
- **Delivery Operations:** Support logistics workflows involving drivers, routes, and delivery records.
- **Responsive Interface:** React-based user interface for logistics management.
- **Database Scripts:** SQL scripts and seed data for setting up the database.

*Note: Feature availability depends on the implemented application workflows and configuration.*

## 🛠️ Tech Stack

### Frontend
- React.js
- Vite
- Tailwind CSS
- Axios
- React Router
- React Leaflet

### Backend
- Java 21
- Spring Boot
- Spring Security
- Spring Data JPA / Hibernate
- JWT
- Maven
- REST APIs

### Database
- PostgreSQL
- SQL

## 🏗️ Project Architecture

```text
ShipTrack Pro
│
├── frontend/       React + Vite application
├── backend/        Spring Boot REST API
├── database/       PostgreSQL schema and seed scripts
├── README.md       Project documentation
└── MILESTONE_1.md  Project milestone documentation
```

### Request Flow

```text
React Frontend
      |
      | HTTP / REST API
      v
Spring Boot Backend
      |
      ├── Spring Security / JWT
      ├── Controllers and Services
      └── Spring Data JPA
                |
                v
           PostgreSQL
```

## ⚙️ Prerequisites

Install the following before running the project:

- Git
- Node.js and npm
- Java Development Kit (JDK) 21
- PostgreSQL
- A code editor such as Visual Studio Code

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/Singh-Vedant/ShipTrack-Pro.git
cd ShipTrack-Pro
```

### 2. Configure the Database

1. Start PostgreSQL.
2. Create a database named `shiptrack`, unless your configuration specifies a different name.
3. Review the SQL files in the `database/` directory.
4. Execute the schema scripts and required seed scripts in the appropriate order.

Check the project's database configuration before running the scripts.

### 3. Configure the Backend

1. Open the `backend/` directory.
2. Review `backend/.env.example`, if available.
3. Create your local `backend/.env` file using the example as a guide.
4. Configure your PostgreSQL connection, credentials, JWT settings, and any other required service credentials.

**Security:** Never commit real passwords, API keys, JWT secrets, or other sensitive credentials.

### 4. Run the Backend

From the project root, run:

```bash
cd backend
chmod +x mvnw
./mvnw spring-boot:run
```

The backend starts using the port configured in the application settings.

### 5. Run the Frontend

Open a second terminal and run:

```bash
cd frontend
npm install
npm run dev
```

Open the local URL printed by Vite in your browser.

### 6. Verify the Application

- Confirm the backend starts without configuration errors.
- Confirm PostgreSQL is connected.
- Open the frontend in your browser.
- Test the authentication and shipment workflows that are configured in your environment.

## 📂 Database

The `database/` directory contains SQL scripts for application tables, relationships, migrations, and sample data.

Review the individual scripts before executing them, especially if you already have data in your database.

## 🔐 Environment Variables

Store environment-specific configuration in local environment files. Use the supplied example files to identify the required variables. Keep local `.env` files and production secrets out of version control.

## 📌 Project Status

ShipTrack Pro is an actively developed full-stack logistics project. Available workflows and deployment requirements may vary with the current implementation.

## 👨‍💻 Author

**Vedant Singh**

- GitHub: [Singh-Vedant](https://github.com/Singh-Vedant)
- LinkedIn: [Vedant Singh](https://www.linkedin.com/in/vedant-singh-03b72832b/)

---

If you find this project useful, consider giving the repository a star ⭐
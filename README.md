# Bidirectional Data Ingestion Between Flat Files and ClickHouse

This project enables bidirectional data ingestion between flat files (e.g., CSV, TSV) and ClickHouse. It supports dynamic configurations for both source and target types, making it flexible for various use cases.

## Requirements

### Backend
- **Java 17 or higher**
- **Maven 3.6+**
- **ClickHouse Database**
- **Spring Boot 2.7.5**

### Frontend
- **Node.js 16+**
- **pnpm** (or npm/yarn)
- **React 18**
- **Next.js**

## Setup Instructions

### Backend
1. Navigate to the `backend` directory:
   ```bash
   cd backend
   ```
2. Build the project using Maven:
   ```bash
   mvn clean install
   ```
3. Run the Spring Boot application:
   ```bash
   mvn spring-boot:run
   ```
4. The backend will start on `http://localhost:8080` by default.

### Frontend
1. Navigate to the `frontend` directory:
   ```bash
   cd frontend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   npm run dev
   ```
4. The frontend will start on `http://localhost:3000` by default.

## Features
- **Ingestion**: Supports data ingestion from ClickHouse to flat files and vice versa.
- **Dynamic Configuration**: Allows users to configure source and target types dynamically.
- **Preview**: Provides a preview of data before ingestion.
- **JWT Authentication**: Securely connects to ClickHouse Cloud using JWT-based authentication.

## Usage
1. Open the frontend in your browser at `http://localhost:3000`.
2. Follow the multi-step UI to configure the source and target types.
3. Preview the data and select columns for ingestion.
4. Trigger the ingestion process and view the results.

## Testing
### Backend
Run the tests using Maven:
```bash
mvn test
```

## Contributing
1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Submit a pull request with a detailed description of your changes.

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.
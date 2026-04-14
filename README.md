# Travel Management System

A Java Swing based desktop application for managing travel and tourism operations.

## Setup Instructions

### Prerequisites
- **Java Development Kit (JDK):** Version 8 or higher
- **Database:** MySQL Server
- **IDE:** NetBeans (Recommended) or you can run using standard Java tooling.

### Installation

1. **Clone the Repository**
   ```bash
   git clone <repository_url>
   cd "Travel Management System"
   ```

2. **Add Required Libraries**
   This project relies on the following external libraries. You will need to download them and place them in a `lib/` folder at the root of the project:
   - `mysql-connector-java.jar` (MySQL JDBC Driver)
   - `rs2xml.jar` (Used for converting ResultSet to xml/tables)

   Create a `lib/` directory:
   ```bash
   mkdir lib
   ```
   And place the downloaded `.jar` files inside `lib/`.

3. **Database Configuration**
   - Create a MySQL database (e.g., `travelmanagementsystem`).
   - Import the required SQL schema or create the tables (refer to standard application setup if SQL file provided).
   - Update the database connection credentials in the `Conn.java` or `Connection` utility class with your MySQL username and password.

4. **Build and Run**
   If using NetBeans:
   - Open the project in NetBeans.
   - Right-click the project -> Resolve Missing Dependencies (point to the jars in your `lib/` folder if prompted).
   - Run the project.

   If using Command Line:
   ```bash
   javac -cp "lib/*" src/travel/management/system/*.java
   java -cp "lib/*;src" travel.management.system.Login
   ```

## License
MIT License

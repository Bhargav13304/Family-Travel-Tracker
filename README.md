# Family Travel Tracker

A web application designed to help families track and visualize the countries each member has visited. Users can add family members, assign them unique colors, and mark visited countries on an interactive world map.

## Features
- **User Management:** Add and manage family members with distinct color indicators.
- **Country Tracking:** Track and display visited countries for each family member.
- **Interactive Map:** Visual representation of visited countries.
- **Dynamic Data Handling:** Data fetched and managed using PostgreSQL.

## How It Works
- **Home Page:** Displays all family members and their assigned colors. The total number of visited countries is shown as well.
- **Adding a Family Member:** Users can add new family members by clicking the "Add New Member" button, specifying their name and preferred color.
- **Switching Users:** Select a family member to view their visited countries and continue adding more.
- **Adding Visited Countries:** Users can type in a country name, and if valid, it will be added to that family member's visited list.

## Technologies Used
- **Frontend:**
  - HTML
  - CSS
  - EJS (Embedded JavaScript)  
- **Backend:**
  - Node.js
  - Express.js
- **Database:**
  - PostgreSQL
- **Middleware:**
  - body-parser
- **Libraries & Tools:**
  - pg (PostgreSQL client for Node.js)
- **Other References:**
  - `countries.csv` for country data
  - `.env` for environment variables configuration

## Project Structure
```
/Family-Travel-Tracker
├── /public          # Static files (CSS, Images)
├── /views           # EJS templates
├── solution.js      # Main server logic
├── queries.sql      # Database setup commands
├── countries.csv    # Dataset for country codes
└── .env             # Environment variables for database credentials
```

## Installation and Setup
1. **Clone the repository:**
   ```bash
   git clone https://github.com/Bhargav13304/Family-Travel-Tracker.git
   cd Family-Travel-Tracker
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Set up the PostgreSQL database:**
   - Install PostgreSQL if not already installed.
   - Create a database named `world`.
   - Execute the SQL commands provided in `queries.sql` to set up tables.
   - Import `countries.csv` into the appropriate table (ensure header option is enabled).

4. **Configure environment variables:**
   - Create a `.env` file in the root directory.
   - Add the following details:
     ```env
     DB_USER=your_postgresql_username
     DB_PASSWORD=your_postgresql_password
     DB_NAME=world
     DB_HOST=localhost
     DB_PORT=5432
     ```

5. **Start the application:**
   ```bash
   node solution.js
   ```

6. **Access the application:**
   - Open your browser and visit `http://localhost:3000`


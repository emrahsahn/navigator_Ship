# navigator_ship
# Navigator Ship Database

This project is a Python application simulating a ship management system using SQLite. The application allows recording, updating, deleting, and viewing different types of ships, employees, and expeditions. The application uses the `tkinter` library for the user interface.

### Ship Types:
- `CRUISE_SHIP`: Passenger ship
- `OIL_SHIP`: Oil tanker
- `CONTAINER_SHIP`: Container ship

### Employee Types:
- `CAPTAIN`: Captain
- `CREW`: Crew

### Harbor-Related Classes:
- `HARBOR`: Harbor information
- `VISITED_HARBORS`: Visited harbors

### Expeditions:
- `EXPEDITIONS`: Expedition information

### Interface:
- `Add Record`: Adds a new record.
- `Delete Record`: Deletes an existing record.
- `Update Record`: Updates an existing record.
- `View Table`: Views a table.
- `Close`: Closes the application.

### Structure:

#### Classes:
- `SHIP`: Main ship class (User cannot access).
- `CRUISE_SHIP`, `OIL_SHIP`, `CONTAINER_SHIP`: Subclasses for ship types.
- `EMPLOYEE`: Main employee class (User cannot access).
- `CAPTAIN`, `CREW`: Subclasses for employee types.
- `HARBOR`, `VISITED_HARBORS`, `EXPEDITIONS`: Classes related to harbors and expeditions.

#### Functions:
- `_construct_main_menu()`: Constructs the main menu.
- `_construct_menu(action)`: Constructs the submenu.
- `_handle_input(textBox, sampleTable, action, classType, c)`: Takes input from the user and calls the relevant function.
- `insert_sample(sampleTable, sampleAttrs, classType, c)`: Adds a new record.
- `delete_sample(sampleTable, sampleAttrs, classType, c)`: Deletes an existing record.
- `update_sample(sampleTable, sampleAttrs, c)`: Updates an existing record.
- `display_table(sampleTable)`: Views a table.

#### Database Connection:
- `conn = sql.connect('navigatorShip.db')`: Creates the database connection.
- `c = conn.cursor()`: Creates the database cursor.

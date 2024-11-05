# Ship Management System

## Project Description
This project is developed as part of the Database Management Systems course and is designed for the "Gezgin Ship Company" to manage voyages with different types of ships. The software manages data related to:

- Ships
- Voyages
- Captains
- Crew Members
- Harbors

The company operates various types of ships including passenger ships, oil tankers, and container ships. For each ship, the system stores a unique serial number, name, weight, and year of manufacture. Additional attributes specific to each type are also stored:
- **Passenger ships**: Passenger capacity
- **Oil tankers**: Oil capacity in liters
- **Container ships**: Number of containers and maximum weight capacity

Each ship can embark on multiple voyages over time, with each voyage limited to one ship at a time. A minimum of two captains and one crew member is required for each voyage. The voyage records include an ID, departure date, return date, and departure harbor. A voyage can dock at multiple harbors, and the company wishes to keep records of past voyages, planned future voyages, and potential voyages.

Each harbor may be visited by multiple ships over different voyages. For each harbor, the system stores the harbor name, country, population, passport requirement, and docking fee. The harbor name and country are unique identifiers. Additionally, records of harbors that have not yet been visited but may be in the future can be added to the database.

For captains and crew members, the system stores ID, first name, last name, address, nationality, date of birth, and hiring date. Additionally, captains have license details, and crew members have their specific roles recorded. Captains and crew members can only be assigned to one voyage at a time.

The project requires the development of a form-based application where users can add, delete, and update the information described above. The data should be stored in a SQL Server database and managed via object-oriented programming (OOP) principles. Classes should be created for each entity, with operations related to each entity handled through instances of these classes. Database tables should be created for each entity, ensuring data is stored correctly. All database operations should be managed within the software.

---


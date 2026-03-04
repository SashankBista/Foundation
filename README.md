# Student Club Database Management System

## Task 3: Normalization & ER Diagramming
This repository contains the database implementation for a Student Club system, evolved from a flat-file structure into a fully normalized **Third Normal Form (3NF)** schema.

### Normalization Logic
1. **2NF Implementation**: Separated the data into `Students` and `Clubs` to remove partial dependencies.
2. **3NF Implementation**: Ensured that all non-key attributes (like `ClubMentor` or `Email`) depend solely on their respective Primary Keys (`ClubID` or `StudentID`), removing transitive dependencies.

### ER Diagram
The ER Diagram (found in the `/diagrams` folder) illustrates the **Many-to-Many** relationship between Students and Clubs, mediated by the `Membership` associative entity.
- **Cardinality**: One Student -> Many Memberships; One Club -> Many Memberships.

### SQL Operations 
- **Schema Creation**: Tables are built with Foreign Key constraints to maintain referential integrity.
- **Join Operations**: A three-way join is used to reassemble the normalized data into a human-readable report showing Student Name, Club Name, and Join Date.

### Task 6: Reflection
- **Redundancy**: Normalization reduced data repetition by storing club details (Room/Mentor) only once.
- **Accuracy**: Data integrity is improved by preventing update anomalies; changing a club's room now only requires a single row update.

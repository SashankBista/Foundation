# Computer Science Foundations: Task Portfolio

This repository contains the practical implementations for Tasks 1, 2, and 3.

## Task 1: Secure Data Exchange
- **Focus**: Encoding formats (Base64, Hex, URL) and Protocol security (TLS/HTTPS/SMTP).
- **Files**: See `/Task_1_Secure_Data_Exchange` for diagrams showing data flow and encoding-based obfuscation risks.

## Task 2: Classroom Seating Arrangement (P vs NP)
- **Problem**: Arranging students based on friendship and city constraints.
- **Complexity Analysis**: 
  - **P vs NP**: Verification is O(n), discovery is O(n!).
  - **Heuristics**: Implementation of "Most Constrained First" strategies to reduce search time.
- **Visuals**: `/Task_2_Seating_Problem/complexity_graph.png` illustrates the growth of n! vs polynomial time.

## Task 3: College Club Membership Management
This section demonstrates full Database Normalization (1NF to 3NF).

### Normalization Steps:
1. **1NF**: Atomic values confirmed; Composite Primary Key established.
2. **2NF**: Separation of Student and Club entities to remove partial dependencies.
3. **3NF**: Removal of transitive dependencies (e.g., ClubRoom/Mentor tied strictly to ClubID).

### SQL Scripts:
- Found in `/Task_3_Database_Management/schema_and_queries.sql`.
- Includes Schema creation, Data insertion, and a 3-way JOIN query.

### ER Diagram:
- Found in `/Task_3_Database_Management/ER_Diagram.png`.
- **Entities**: Students, Clubs, Membership.
- **Relationship**: Many-to-Many (M:N) mediated by an associative table.

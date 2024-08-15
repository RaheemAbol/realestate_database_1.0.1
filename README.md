### Ticket Breakdown

#### **Ticket 1: Setup the Real Estate Database**
- **Tasks:**
  - Set up the database using the provided SQL script.
  - [Download healthcare_system.sql](https://raw.githubusercontent.com/RaheemAbol/realestate_database_1.0.1/main/realestate_database.sql)
  - Ensure that all tables are created, and data is inserted correctly.

#### **Ticket 2: INNER JOIN**
- **Tasks:**
  1. **List all properties along with the agent's first name, last name, city, and state.**
     - Use an INNER JOIN between the `Properties` and `Agents` tables.
  2. **Retrieve the transaction ID and the associated property address, city, and state.**
     - Use an INNER JOIN between the `Transactions` and `Properties` tables.
  3. **Find all properties listed by a specific agent (e.g., AgentID = 3) along with the property address, city, state, and listing price.**
     - Use an INNER JOIN between the `Properties` and `Agents` tables.
  4. **List all clients along with their first name, last name, email, and the properties they have purchased (address, city, state).**
     - Use an INNER JOIN between the `Transactions`,`Properties` and `Clients` tables.

#### **Ticket 3: LEFT JOIN**
- **Tasks:**
  1. **List all agents, including their first name, last name, email, and phone number, along with the properties they have listed (include property address, city, and state), even if they have no listings.**
     - Use a LEFT JOIN between the `Agents` and `Properties` tables.
  2. **Retrieve all properties, including the property address, city, state, and listing price, along with their transaction details (transaction ID and sale price), even if the property has not been sold yet.**
     - Use a LEFT JOIN between the `Properties` and `Transactions` tables.
  3. **List all clients, including their first name, last name, email, and phone number, along with the properties they have purchased (include property address, city, and state), even if they haven't purchased anything.**
     - Use a LEFT JOIN between the `Clients` and `Transactions` tables.
  4. **Retrieve all property types (e.g., Single Family, Condo), including the type name and the details of properties listed under each type (address, city, state), even if no properties are listed under that type.**
     - Use a LEFT JOIN between the `PropertyTypes` and `Properties` tables.

#### **Ticket 4: RIGHT JOIN**
- **Tasks:**
  1. **List all properties, including their address, city, state, and listing price, along with the assigned agent's first name, last name, and email, even if the property doesn't have an assigned agent.**
     - Use a RIGHT JOIN between the `Properties` and `Agents` tables.
  2. **Retrieve all transactions, including transaction ID, sale price, and sale date, along with the client's first name, last name, email, and phone number, even if the transaction doesn't have an associated client.**
     - Use a RIGHT JOIN between the `Transactions` and `Clients` tables.
  3. **List all property types, including the type name, and the details of properties listed under each type (address, city, state), even if no properties are listed under that type.**
     - Use a RIGHT JOIN between the `Properties` and `PropertyTypes` tables.
  4. **List all clients, including their first name, last name, email, and phone number, along with the transaction ID and sale date, even if they haven't made any transactions.**
     - Use a RIGHT JOIN between the `Transactions` and `Clients` tables.

#### **Ticket 5: CROSS JOIN**
- **Tasks:**
  1. **Create a list of all possible combinations of agents and properties, including the agent's first name, last name, and email, along with the property address, city, state, and listing price.**
     - Use a CROSS JOIN between the `Agents` and `Properties` tables.
  2. **Generate a list of all possible client and property combinations, including the client's first name, last name, and email, along with the property address, city, state, and listing price.**
     - Use a CROSS JOIN between the `Clients` and `Properties` tables.
  3. **Create a list of all property types and all properties, including the type name, property address, city, state, and listing price.**
     - Use a CROSS JOIN between the `PropertyTypes` and `Properties` tables.
  4. **List all agents with all clients they could potentially serve, including the agent's first name, last name, and email, along with the client's first name, last name, and email.**
     - Use a CROSS JOIN between the `Agents` and `Clients` tables.

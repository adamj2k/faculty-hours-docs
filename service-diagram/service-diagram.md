# Services
### Gateway
Acts as the entry point for external requests. It handles authentication using Auth0 and routes requests to the appropriate microservices.  
### Faculty Service
Manages faculty-related operations and data. It interacts with a PostgreSQL database to store and retrieve faculty information.  
### Broker
Facilitates communication between services by sending and consuming messages. It is utilized to trigger events such as faculty data changes.  
### Report Service
Generates reports based on data received from the Faculty service. It consumes messages from the Broker and stores report data in a MongoDB database.   
### Payrolls Service
Manages payroll operations, interacting with a PostgreSQL database to process and store payroll data.  
## Data Flow
External Requests: Users send HTTP requests to the Gateway, which authenticates and routes them.  
Faculty Operations: The Faculty service processes faculty-related requests and communicates changes via the Broker.  
Event Handling: The Broker sends messages to the Report service when faculty data changes.  
Report Generation: The Report service consumes messages and updates the MongoDB database with new reports.  
Payroll Processing: The Payrolls service handles payroll data requests and updates the PostgreSQL database accordingly.  
## Technologies Used
Auth0: For authentication.  
RabbitMQ: For message brokering.  
PostgreSQL & MongoDB: For data storage.  
FastAPI & SQLAlchemy: For API and ORM.  
Docker: For containerization.  
## Prerequisites
Python 3.11 or higher  
Docker and Docker Compose  
Poetry package manager  
PostgreSQL and MongoDB databases  


# faculty-hours-docs
Documentation for faculty-hours app as microservice app

## Description
### General info
This application has been built as an example of a microservices-based application. Its purpose is to support the management of teacher workload in a university department by collecting data about the classes taught, generating reports and payroll that can be shared with other external services.

### Services:
#### faculty-hours-gateway
 - Gateway API for Project Faculty Hours
####  faculty-hours-faculty
 - CRUD service to manage subject, exercise and teachers on Faculty
#### faculty-hours-raport
 - Service for the reporting of the status of the subjects of the faculty and the teaching loads of the faculty members.
#### faculty-hours-broker
 - Broker for automatic triggering of report generation when data in the database changes.
#### faculty-hours-payrolls
 - Service for creating payrolls based on data obtained from reports.

### Tech-stack
Python 3.11  
FastAPI  
Pandas  
  
<u>Database:</u>  
PostgreSQL  
MongoDB  
  
<u>Code Quality and Development Tools:</u>  
Black (code formatter)  
isort (import sorter)  
Poetry (dependency management)  
  
<u>Deployment:</<u>  
Docker Compose (local)  


### Setup

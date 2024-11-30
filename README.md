# faculty-hours-docs
Documentation for faculty-hours app as microservice app

## Description
### General info
This application has been built as an example of a microservices-based application. Its purpose is to support the management of teacher workload in a university department by collecting data about the classes taught, generating reports and payroll that can be shared with other external services.

### Services:
#### faculty-hours-gateway
 - Gateway API for Project Faculty Hours
 - [link to repo](https://github.com/adamj2k/faculty-hours-gateway)
####  faculty-hours-faculty
 - CRUD service to manage subject, exercise and teachers on Faculty
 -  [link to repo](https://github.com/adamj2k/faculty-hours-faculty)
#### faculty-hours-raport
 - Service for the reporting of the status of the subjects of the faculty and the teaching loads of the faculty members.
 - [link to repo](https://github.com/adamj2k/faculty-hours-raport)
#### faculty-hours-broker
 - Broker for automatic triggering of report generation when data in the database changes.
 - [link to repo](https://github.com/adamj2k/faculty-hours-broker)
#### faculty-hours-payrolls
 - Service for creating payrolls based on data obtained from reports.
 - [link to repo](https://github.com/adamj2k/faculty-hours-payrolls)

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

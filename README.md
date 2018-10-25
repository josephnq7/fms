# Online Support

## Introduction
	We are going to design and implement a online Flight Management and Booking project. This is an engineering proof of concept. It is not a planned marketable project. 
	The goal is to exercise the Spring MVC technology according to the Web Application Architecture (WAA) course guidelines to validate its use in future projects.

## Purpose
	Online Flight Management and Booking is a web application which provides users the ability to view and make booking for a flight online. Once the booking is made, user can be able to view their booking information by providing the system their confirmation code [auto generated after successful] for security check. 
	The system also provides back-office features for system administration purpose. These features are provided for authorized persons only. Who have to provide username and password for authentication & authorization 

## Requirements
- View scheduled flights
- Create, Update Airline, Airport, Airplane
- Schedule new flight
- Online support
- Create & View flight booking 

## Main Use-Cases
### [Admin]Login
- Admin click login button on the web page
- System show the login form
- Admin enter username and password
- Admin click on the Login
- System validates and performs authentication for provided login credential
- System performs authorization if authenticated user has admin role
- System display admin's home page

### [Admin]Logout
- Admin click logout button on the web page
- System log the user out
- System clear all resources of logged out user

### [Admin]Schedule new flight
- Admin click Schedule New Flight button on the web page
- System show the New Flight form
- Admin enter all required fields from the form (e.g. name, departure city/date/time, arrival city/date/time...)
- Admin click on the Save
- System validates all required fields
- System saves data to the database and show the detail of new scheduled flight

### [Admin]Edit existed flight
- Admin click Edit button on the web page
- System show the Flight form
- Admin modify fields on the form (e.g. name, departure city/date/time, arrival city/date/time...)
- Admin click on the Save
- System validates all required fields
- System saves modified data to the database and show the detail page of updated flight

### [Admin] create new Airpline
- Admin click on New Airline
- System shows New Airline form
- Admin enter airline information
- Admin click Save
- System validates input data and save airline to the database and display detail page of added airline 

### [Admin] update Airpline
- Admin click on Edit button
- System shows Airline form
- Admin modify fields on the form 
- Admin click Update
- System validates input data and update modified airline to the database and display detail page of modified airline 

### [Admin] create new Airplane
- Admin click on New Airplane
- System shows New Airplane form
- Admin enter Airplane information
- Admin click Save
- System validates input data and save Airplane to the database and display detail page of added Airplane

### [Admin] update Airplane
- Admin click on Edit button
- System shows Airplane form
- Admin modify fields on the form 
- Admin click Update
- System validates input data and update modified Airplane to the database and display detail page of modified Airplane 

### [Admin] create new Airport
- Admin click on New Airport
- System shows New Airport form
- Admin enter Airplane information
- Admin click Save
- System validates input data and save Airport to the database and display detail page of added Airport 

### [Admin] update Airport
- Admin click on Edit button
- System shows Airport form
- Admin modify fields on the form 
- Admin click Update
- System validates input data and update modified Airport to the database and display detail page of modified Airport 

### User make a booking
- User search and select a flight
- System display detail flight information
- User clicks on Make Reserve
- System display detail flight information and start booking flow
- User provides required data follow the reservation flow defined by the system
- At the last step of booking flow, user click on Confirmation
- System saves collected reservation data from user to the database
- System display Thank You page with confirmation code of the booking 

### User view a booking
- User click on My Booking
- System display booking page
- User enters data (e.g. confirmation code) and click on View
- System display detail booking information


## Class Diagram

## Sequence Diagrams

### For User
- Make a booking
- View booking detail
- Call online support

### For Admin user
- Login & Logout
- Create & Update Airline, Airplane, Airport
- Schedule and Update flight
- Online support user

## Technologies Used
- Annotation
- Data binding
- Validation; Custom Validation
- Custom Formatter, Custom Interceptor
- Internationalization
- Exception Handling
- REST/Ajax two way; error handling
- Security; Authentication & Authorization
- Web Sockets
- Web Flow
- Tiles
- Persistence in database [JPA]
- DB: MySQL

## Tools
- Spring Tool Suite 4
- Maven
- GitHub

## Project Guidelines
### Setup MySQL
- Create MySQL database schema "saigonese"
- Grant schema previleges to root user
- You may have to update username/password in "src/webapp/WEB-INF/spring/context/applicationContext.xml" [default used in the project: "root/root"]

### To run the project
- Import source into STS
- Update project Maven dependencies (you may have to config add Maven dependencies into Deployment Assembly)
- Build and run
- "admin/admin" is default username/password for loging to admin back-office





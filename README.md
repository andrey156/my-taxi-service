# my-taxi-service
DESCRIPTION
This is a taxi service project that provides essential functionalities for managing drivers, cars, and manufacturers. Users can perform actions such as adding new drivers and cars, assigning drivers to vehicles, and accessing detailed information about drivers, cars, and manufacturers.

FEATURES
Authentication, Display current cars, Display all drivers, Display all cars, Display all manufacturers, Add driver to car, Add new driver, Add new car, Add new manufacturer.

STRUCTURE

Controllers:
Authentication controllers:
1.	LoginController
2.	LogoutController

Car controllers:
1.	AddCarController
2.	AddDriverToCarController
3.	DeleteCarController
4.	GetAllCarsController

Driver controllers:
1.	AddDriverController
2.	DeleteDriverController
3.	GetAllDriversController
4.	GetMyCurrentCarsController

Manufacturer controllers:
1.	AddManufacturerController
2.	DeleteManufacturerController
3.	GetAllManufacturersController
4.	IndexController: Home page ("/index")

Data Access Objects (DAOs):
1.	CarDaoImpl
2.	DriverDaoImpl
3.	ManufacturerDaoImpl

Exceptions:
1.	AuthenticationException
2.	DataProcessingException

Models:
1. Car
2.	Driver
3.	Manufacturer

Services:
1.	AuthenticationServiceImpl
2.	CarServiceImpl
3.	DriverServiceImpl
4.	ManufacturerServiceImpl

Utilities:
1.  ConnectionUtil

Resources:
1.	init_db.sql (SQL script to initialize the database)
2.	Webapp: JSP files, CSS file, web.xml configuration file


To run the application, ensure that you meet the following prerequisites:
1.  Java 11 or later
2.  Apache Tomcat 9 (recommended version: 9.0.73)
3.  MySQL 8 or later

To set up the project:
1.	Clone the project repository.
2.	Execute the SQL script in src/main/resources/init_db.sql to initialize the database.
3.	Update the database configuration in src/main/java/util/ConnectionUtil.
4.	Build the project using Maven: mvn clean package.
5.	Deploy  the generated WAR file to your servlet cantainer.
6.	Use   http://localhost:8080

TECHNOLOGIES
1.  Maven v.3.10.1: Build tool and dependency management.
2.  JDK v.11.0.2: Java Development Kit.
3.	MySQL v.8.0.22: Relational database management system.
4.	Tomcat v.9.0.73: Server for deploying Java web applications.
5.	Java Servlets v.4.0.1: Technology for developing web applications in Java.
6.	JDBC v.4.2: Java Database Connectivity.
7.	JSTL v.1.2: JavaServer Pages Standard Tag Library.
8.	JSP v.2.3: JavaServer Pages.
9.  HTML v.4.01: HyperText Markup Language.


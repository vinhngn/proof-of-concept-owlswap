
**Please make sure to have those installed:**
* MySQL Server & MySQL Workbench 
* Java JDK 
* Apache Maven 
* Node.js
  
**How to run:**
	Navigate to the root directory of the project 
			cd proof-of-concept
   
**Establish Database: **
* Launch the installed mySQL Workbench 
* Connect to the MySQL Server using the previously created account
* Create a database named testing
  
**Running tha Back-end: **
(1) Navigate to the backend/directory
	cd backend
(2) Before running the below command, please check the file named application.properties to check the code below:
      spring.datasource.url=jdbc:mysql://localhost:3306/testing?useSSL=false&serverTimezone=UTC
      spring.datasource.username=root
      spring.datasource.password=123123xx
(3) Make the the localhost port in mySQL the same, otherwise modify 3306 to the corresponding
       + Check username
       + Change password if needed
(4) Run the following command to start the back-end server: 
		  mvn spring-boot:run
(5) Back-end run successfully on port 8080 
(6) Return to the root directory of the project
	  	cd ..
  
**Running the Front-end: **
(1) Navigate to the frontend/ directory:
	  cd frontend
(2) Run the following command to install the necessary dependencies: 
	  npm install
(3) Run the following command to start the front-end server:
	  npm start 
(4) Open a web browser and navigate to http://localhost:3000/ to view the application.

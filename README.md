# Student_tracking
This project was designed to allow teachers or administrators to track student attendance and performance using a web interface. The system included both frontend and backend components, utilizing technologies such as HTML, CSS, JavaScript, Node.js, and MySQL.
Setup Guide
Prerequisites
Before running the server, ensure you have the following installed:
•	Node.js: Download and install from Node.js official website
•	MySQL: Download and install from MySQL official website

MySQL Setup
1.	During the installation of MySQL, set the root password to root 
	(or another password of your choice).
2.	If you choose a different password, update it in the server.js file accordingly.
3.	Open the command prompt and access MySQL:
	mysql -u root -p
4.	Enter the password you set during installation.
5.	Add the code from database.sql file.
6.	Don't forget to add users:
	(INSERT INTO users (username, password) VALUES ('your_username', 'your_password');
7.	If there will be a problem with connecting to the DB from server due to the clients
	version, add the following code into the database to change the method of authentication:
	ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'root';
	FLUSH PRIVILEGES;
	
Node.js Setup
1.	Move the server.js file to the user directory:
	C:\Users\User\
2.	Install the required Node.js dependencies through command prompt:
	npm install express mysql body-parser cors
This will install all necessary packages.

Running the Project
1.	Start the server through command prompt:
	node server.js
2.	Open index.html

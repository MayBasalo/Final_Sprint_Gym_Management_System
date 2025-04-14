Final Sprint – Winter 2025
Gym Management System
Project Overview
You have been tasked with developing a console-based Gym Management System using a Maven-based Java project with PostgreSQL. This project will simulate management of a gym, allowing different users—Admins, Trainers, and Members—to interact with the system based on their roles.
The project should be implemented as a team effort, with each group consisting of up to three students. Every team member should actively contribute to the project.
Solos will be considered on a case-by-case basis. 

Project Objectives
•	Develop a Java application that manages gym users, memberships, and workout classes.
•	Implement user authentication and role-based access control (RBAC) for Admins, Trainers, and Members.
•	Integrate the system with a PostgreSQL database to store and manage user, membership, and workout class data.
•	Demonstrate effective teamwork and project management skills using GitHub and other tools.

Functional Requirements
User Registration and Authentication
•	Users can register with a username, password, email,phonenumber,address and role (Admin, Trainer, or Member).
•	Registered users can log in and see a role-specific menu.
•	Passwords must be securely stored using BCrypt hashing. Passwords can be hashed before being saved to the Database (Maven dependency or adding JAR file manually required in order to access BCrypt).
•	Example classes: 
o	User, UserDAO, UserService 
o	Admin, Trainer, Member (Inheritance from User)
Product Management: Memberships & Classes
Membership Management
•	Members and trainers can purchase a gym membership.
•	Admins can view and track total revenue from memberships in the gym.
•	Example classes: Membership, MembershipDAO, MembershipService
Workout Class Management
•	Trainers can add, update, and delete workout classes.
•	Members can view a list of workout classes in the system
•	Example classes: WorkoutClass, WorkoutClassDAO, WorkoutClassService

Role-Based Functionality
Admin
•	View all users in the system, including their contact information.
•	Delete users from the system.
•	View all gym memberships and total annual revenue.
Trainer
•	Create, update, and delete workout classes.
•	View a list of all their assigned classes.
•	Purchase a gym membership for themselves.
Member
•	Browse workout classes.
•	View their total membership expenses.
•	Purchase a new gym membership.
Database Integration
•	Use PostgreSQL to store and manage user, membership, and class information.
•	Implement CRUD operations (Create, Read, Update, Delete) for users, memberships, and workout classes.
•	Recommended database schema can include: 
o	Users table (userId,userName,userAddress,userPhoneNumber,userRole...)
o	Memberships table (membershipID,membershipType,membershipDescription,memberShipCost,memberID)
o	WorkoutClasses table (workoutClassID,workoutClasType,workoutClassDescription,trainerID (a trainer is also a user just a different role)

User Interface
•	Develop a console-based user interface for interaction using a scanner.
•	Provide clear menu options and navigation prompts for users.

Technical Requirements
•	Programming Language: Java
•	Database: PostgreSQL ( If you wanna try another feel free byt PG is recommended) 
•	IDE: IntelliJ IDEA, Eclipse, VS Code, or any preferred Java IDE
•	Version Control: Git/GitHub (Mandatory for submission)
•	Dependency Mangement: Maven or Manually adding Jar files will work. 
Submission Guidelines
Code Submission – 60 Marks
•	Submit the complete source code via GitHub.
•	ZIP FILE SUBMISSIONS WILL NOT BE MARKED. If you need help with GitHub, contact you're  TA.
Database Schema – 5 Marks
•	Provide SQL scripts to create and populate your database.
Documentation – 20 Marks
Prepare a detailed report containing the following sections:
1. User Documentation (Assume this is for a user who bought the program. They might not be too smart- Provide lots of detail) 
•	Overview of the application and how it works and what it does
•	Explanation of all classes and their interactions.
•	Class diagram showing relationships between entities.
•	Instructions on how to start and use the system.
2. Development Documentation
•	Javadoc documentation for key methods and classes.
•	Project directory structure explanation.
•	Build process and dependencies used.
•	How to set up the database for development.
•	How to clone and run the project from GitHub.
3.  Individual Report
•	Submit a short individual report detailing: 
o	Your contributions (PRs, branches worked on, contributions to team).
o	Challenges faced during development (Could be anything) 

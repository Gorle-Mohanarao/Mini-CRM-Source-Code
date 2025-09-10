CRM for Sales Teams
This is a single-file CRM (Customer Relationship Management) application designed for sales teams, built as a take-home project. The application serves as a foundational tool for sales representatives to manage their leads and opportunities, while providing managers with a complete, holistic view of the team's data.

To log in as a manager, you can use the credentials for the manager user that are pre-populated in the code.

Simply enter the following information into the login form:

Email: manager@example.com

Password: password

The application will recognize this user as a manager and grant you access to see all leads and opportunities, regardless of who the owner is.

The entire application—including the frontend UI, core business logic, and data storage—is contained within a single index.html file, demonstrating a complete, full-stack application within a simplified structure.

Project Objectives
This project meets all the core requirements outlined in the case study:

Authentication & Role-Based Access Control (RBAC): Users can log in with a rep or manager role.

Lead Management: Full CRUD (Create, Read, Update, Delete) functionality for leads.

Opportunity Management: The ability to update the stage of an opportunity.

Lead-to-Opportunity Conversion: A seamless workflow to convert a qualified lead into a new opportunity.

Data Filtering: Sales representatives can only view their own leads and opportunities, while managers have access to all data.

Simple Frontend UI: A clean, functional user interface with forms and tables to interact with the data.

Core Features
User Roles
Sales Representative (rep): Can create, edit, and delete their own leads. Can convert their leads into opportunities and view only their own data.

Sales Manager (manager): Can view all leads and opportunities across the team. Can update the stage of any opportunity.

Data Models
The application uses a simplified data model for its core entities:

Users: Each user has a unique ID, a name, and a role (rep or manager).

Leads: Each lead has a unique ID, contact information, a status (e.g., New, Contacted, Qualified), and an ownerId to link it to a specific sales representative.

Opportunities: Each opportunity has a unique ID, a title, a value, a stage (e.g., Discovery, Proposal, Won, Lost), and an ownerId.

Workflows
Authentication: The login process handles user authentication and assigns the appropriate role, which determines the user's data visibility.

Lead Management: The leads page displays a table with all visible leads and provides forms for adding new leads or editing existing ones.

Lead Conversion: A "Convert" button on a lead item automatically updates the lead's status to Qualified and creates a new opportunity record.

Opportunity Updates: The opportunities page allows managers to easily update the stage of any opportunity via a dropdown.

Technical Implementation
Language: JavaScript (ES6+), HTML5, CSS3.

Frameworks/Libraries: The application is built without any external frameworks like React or Vue to demonstrate core web development skills. It uses Tailwind CSS for responsive and modern styling, loaded via a CDN.

Data Storage: Data is persisted using the browser's localStorage for a simple, file-based database alternative. This allows for persistent data without requiring a backend server.

Single-File Architecture: The entire application is self-contained within index.html, making it easy to share, deploy, and review.

How to Run
Since the entire application is a single HTML file, you can run it in a web browser instantly.

Open the index.html file in your preferred web browser (e.g., Chrome, Firefox, Safari).

The application will load in the browser, and you can begin using it immediately.

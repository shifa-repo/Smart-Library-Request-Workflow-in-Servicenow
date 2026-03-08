# Smart-Library-Request-Workflow-in-Servicenow

## Project Description

  This project demonstrates how a library book borrowing process can be automated using the ServiceNow platform. The system allows students to request books online while librarians review and approve or reject the requests.
    The project uses custom tables such as Book and Borrow Request to manage library data and transactions. Students can submit borrow requests, and librarians can manage the book catalog and approve requests through an automated workflow.
    The system also uses Flow Designer to automate the approval process. When a student submits a borrow request, the system sends an approval notification to the librarian. Once approved, the system automatically updates the book status to Issued and notifies the student.
    Additional ServiceNow features such as Reference Qualifiers, UI Policies, Access Control Rules (ACLs), and Reports are used to improve system usability, security, and data analysis.
    This automation helps reduce manual work, improve book tracking, and provide better visibility of library usage.
    
------------------------

##Workflow
Student submits Borrow Request
↓
Borrow Request stored in Borrow Request Table
↓
Approval request sent to Librarian
↓
Librarian approves or rejects request
↓
If approved → Book Status updated to Issued
↓
Student receives notification
↓
Data used to generate Most Borrowed Books Report

----------------

##Project Milestones
#Milestone 1 – Role Creation
* Create roles Student and Librarian.
* Assign appropriate permissions for each role.
* Ensure students can request books and librarians can manage the system.
#Milestone 2 – Table Creation
* Create custom tables:
* Book Table (u_book)
* Borrow Request Table (u_borrow_request)
* Configure fields such as title, author, ISBN, request date, and status.
#Milestone 3 – Reference Qualifier Configuration
* Configure a Reference Qualifier on the Book field in Borrow Request table.
* Allow only books with Status = Available to be selected.
* Prevent students from requesting books that are already issued.
Milestone 4 – Workflow Automation using Flow Designer
* Create a flow called Borrow Request Approval Flow.
* Trigger the flow when a borrow request is created.
* Send approval request to librarian.
* On approval:
  Update Book Status → Issued
  Update Borrow Request Status → Approved
* Send email notification to student.
#Milestone 5 – Access Control and UI Policies
* Implement ACL rules to control access for students and librarians.
* Apply UI Policies to improve form behavior.
* Ensure secure and role-based system access.
#Milestone 6 – Report Creation
* Create a report called Most Borrowed Books.
* Group borrow requests by book.
* Count the number of times each book is borrowed.
----------------
##Technologies Used
* ServiceNow Developer Instance
* Flow Designer
* Reference Qualifier
* UI Policies
* Access Control Rules (ACL)
* Reports and Dashboards
---------
##Demo Video
https://drive.google.com/file/d/1573zLNnO220M79erpggS6WFUjJJWvosD/view?usp=drivesdk
--------
‘Team Project’Naan Mudhalvan Project
Team ID : SWTID-2026-1217
Team Size : 4 
Team Leader : SHIFA S
Team member : SIREEN S 
Team member : THASLIMA BANU A 
Team member : SUMAIYA BEGAM M



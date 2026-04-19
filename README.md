# On-Call Paging App for Android
## Project Description
A.	The proposed term project is an Android-based on-call paging application designed for hospital use.

B.	The purpose of the app is to allow staff to quickly page on call personnel during urgent or emergency situations without relying only on manual phone calls.

C.	The app will provide a centralized way to select the needed role, such as CT technologist, Cath lab team, radiologist, or supervisor, and send a page or alert to the appropriate on-call person.

D.	The project will focus on creating a simple, efficient, and user-friendly communication tool for emergency staffing needs.

---	
## Problem Addressing
A.	In many hospital departments, staff must manually look up on call schedules and place individual phone calls when emergency coverage is needed.

B.	This process can waste time, especially when the first person does not answer or when multiple people need to be contacted.

C.	Delays in reaching the correct staff member may affect workflow, patient care, and response time in urgent situations.

D.	The app addresses this problem by organizing on-call information and making it possible to send a page or alert quickly from one interface.

E.	This project supports the broader idea that modern applications are usually connected and should be designed to support communication, data access, and scalable workflows.

---
## Platform
A.	The primary platform for the app will be Android.

B.	The app will be designed for smartphones and tablets commonly used by hospital staff.

C.	MIT App Inventor can support the early prototype because it is a browser-based tool for building Android apps and testing them without requiring a fully traditional coding environment.

D.	If expanded in the future, the concept could also be adapted for iOS or web access.

---
## Front End and Back End Support
### Front End Support

a.	The front end will include the user interface hospital staff will interact with.

b.	Screens may include login, on-call department selection, staff list, paging screen, and confirmation screen.

c.	The design should be simple and fast because users may be under pressure during emergency situations.
	
### Back End Support
---

a.	The back end will store on call schedules, staff contact information, and paging records.

b.	It may use a cloud-connected database or web services, so data can be updated without reinstalling the app.

c.	A connected back end fits the cloud-ready application concept because the app should separate user interaction from the services and data supporting it.

d.	In a future real-world version, the back end could connect with hospital scheduling systems, secure messaging tools, or directory services.

---
## Functionality
A.	User login or secure staff access

B.	View departments or roles currently on call

C.	Search for staff by role or specialty

D.	Send page or alert to selec ted on call staff members

E.	Receive delivery confirmation

F.	Record date, time, and recipient of each page

G.	Escalation option if the first alert is not answered

H.	Optional future features: shift management, administrator editing tools, priority levels of alerts

---
## Design and Wireframes
###	Screen 1: Login Screen

a.	Username field

b.	Password field

c.	Sign In button

###	Screen 2: Home Screen

a.	Department list

b.	On call categories such as Radiology, Cath lab, Nursing Supervisor

c.	Button to view current on call staff

###	Screen 3: Staff Selection Screen

a.	Contact info for on call employee

b.	Send page button

###	Screen 4: Confirmation Screen

a.	Message that an alert was sent

b.	Time stamp

c.	Retry or escalate option

###	Screen 5: Admin Screen, optional future version

a.	Update on call schedules

b.	Add or remove staff

c.	Review alert log

---

### Version 2.0 (Week 4)

- Set up Android Studio project
  
- Added XML layout (TextView, Button)
  
- Started UI structure
  
- Pushed project to GitHub

## Current Implementation Week 7

The application has been developed into a working multi-screen Android app using Java and Android Studio. The following features are currently implemented:

### Screens
- Login Screen (MainActivity)
- Department Selection Screen (DepartmentActivity)
- Page Type Selection Screen (PageTypeActivity)
- Confirmation Screen (ConfirmActivity)

### Core Features
- User login with basic validation (username and password fields)
- Selection of on-call role:
  - CT Technologist
  - Cath Lab Team
  - Radiologist
  - Supervisor
- Selection of page priority:
  - Routine
  - Urgent
  - Emergency
- Confirmation screen displaying selected role and page type
- Ability to send:
  - SMS messages using Android Intent
  - Email messages using Android Intent
- Navigation between screens using Intents
- Back navigation to return to department selection

### App Flow
Login → Department Selection → Page Type → Confirmation → Send Page

### Technical Concepts Used
- Java programming
- Android Activities and lifecycle
- Intents for screen navigation
- Implicit Intents for SMS and Email
- XML layouts for UI design
- Toast messages for user feedback

### Limitations
- No real backend or database connection
- Contact information is not dynamically stored
- SMS and Email rely on external apps
- No authentication validation beyond basic input checking

### Future Improvements
- Connect to a real backend database for on-call schedules
- Add secure authentication
- Store and manage contact information dynamically
- Add escalation logic if no response is received


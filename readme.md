
# **PART B DOCUMENTATION**

## Links

All repositories:

https://github.com/Final-Full-Stack-Project-Team

# **Testing the backend**	

There are 4x collections in the database. The collections are:
- groups
- items
- lists
- users

The screenshots below show testing for all CRUD functionality of the backend.

## Groups Collection

### Users

*User Sign up*

User sign up requires the name field to not be blank, the email address to meet requirements (cannot contain spaces, must contain '@' and '.') and the password to meet requirements (contain at least 8 characters, a capital letter, and a number)

When name is blank:
![Alt text](docs/Backend-testing/Users/Sign-up-blank-name.png)

When email contains a space, does not contain a '@', '.' or is blank:
![Alt text](docs/Backend-testing/Users/Sign-up-bad-email.png)

When password does not contain at least 8 characters, a capital letter, and a number:
![Alt text](docs/Backend-testing/Users/Sign-up-bad-password.png)

When signup is successful:
![Alt text](docs/Backend-testing/Users/Sign-up-success.png)

*User Login*

User login requires correct username and password. 

When logging in with incorrect credentials:
![Alt text](docs/Backend-testing/Users/Login-invalid.png)

When logging in successfully:
![Alt text](docs/Backend-testing/Users/Login-success.png)


*GET users*

GET all users:
![Alt text](docs/Backend-testing/Users/Get-all-users.png)

GET user with id:

When getting user with invalid ID:
![Alt text](docs/Backend-testing/Users/Get-user-not-found.png)

When getting user with a valid ID:
![Alt text](docs/Backend-testing/Users/Get-user-success.png)







<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>

# **PART A DOCUMENTATION**
# **R1**
## Description of your website, including: Purpose, Functionality / features, Target audience, Tech stack


### Purpose:
The purpose of the app is to provide users with an effective and easy-to-use solution for sharing and collaborating on lists. Lists are used for many varying applications such as a grocery list, a to-do list, a travel itinerary, a to-do list and more. This app aims to streamline the process of creating, sharing, and managing lists among multiple users with ease. It aims to have a clean UI and UX that makes sense without a steep learning curve so the user can efficiently use the list right away.

### Functionality / Features:

The app aims to have the following features. Although during development, things may change:

- User signup using bcrypt for passwords.

- User sign in page with password reset option.

- Once a user successfully signs up for an account they can create shared groups and add people to them via email. Groups are an optional feature which is useful for users who frequently share lists with the same people. A user can also invite people directly via email without the need to create a group.

- Users can create, read, update and delete new lists.

- Once a list is no longer needed it can be marked as completed.
There will be a "completed" section of the app where completed lists can be read, marked as active, or be deleted.

- All people with access to a list can add items and cross them off the list with a checkbox.

- Crossing items off the list adds a line through the text and ticks the checkbox for easy visual confirmation.

- User accounts, user groups, lists and list items are stored in individual MongoDB collections.

- Multiple users can collaborate on the same list simultaneously, adding items, crossing out completed tasks, and making real-time updates. This feature promotes teamwork and ensures everyone stays on the same page, literally.

### Target Audience:
The app's target audience is any individual or group of people who frequently need to create and manage shared lists. It caters to users of all ages and technical backgrounds, aiming to provide a user-friendly experience for both tech-savvy individuals and those less familiar with technology.

### Tech Stack:
The app utilizes a modern tech stack to deliver a seamless and responsive user experience:

Front-end: HTML, CSS, JavaScript, React.js
<br>
Back-end: Node.js, Express.js
<br>
Database: MongoDB
<br>
Hosting: Netlify, MongoDB Atlas
<br>
Authentication: JWT (JSON Web Tokens)


# **R2**	
## Data Flow Diagrams

![UserOperationsDataDiagram](./docs/User-Data-Operations.jpg)
![GroupOperationsDataDiagram](./docs/Group-Data-Operations.jpg)
![ListOperationsDataDiagram](./docs/List-Data-Operations.jpg)
![ItemOperationsDataDiagram](./docs/Item-Data-Operations.jpg)

# **R3**	
## Application Architecture Diagram

![ArchitectureDiagram](./docs/Architechture-diagram.jpg)

# **R4**	
## User Stories

1. As an active business person, I want to be able to quickly create lists when I'm on the go and share them with my colleagues so we can keep track of deadlines and prioritize tasks while collaborating efficiently.

2. As a student, I want to be able to share lists with my cohorts so that we can  work together on upcoming group assignments and check off the list as they are completed in order to stay up-to-date on what tasks are ahead of us.

3. As a parent, I want to be able to create weekly grocery lists that can be easily edited while at the supermarket as my grocery needs frequently change. I want to share this list with my partner so they can add items to the list that I may have forgotten.

4. As a traveling salesperson I want to be able to create a list of clients and be able to mark them as completed or crossed out so that I can keep track of the clients who I have visited on any given day.

5. As a person who is not highly tech savvy, I would like to be able to create to-do lists in an app that is simple to use so that I can focus on my tasks without getting overwhelmed by complex user interfaces.

6. As a camping enthusiast, I want to make an inventory of all of my camping gear so that I can check that I have everything I need before heading off to my next camping adventure. After my camping trip has finished, I want to be able to quickly uncheck all items on the list so that I can go through the list again for future trips. I want to be able to easily edit and delete items when I buy or replace things.


# **R5**	
## Wireframes for multiple standard screen sizes, created using industry standard software

The below working file contains wireframes/designs for mobile, tablet and desktop. In the mobile design, the relationship between each page is outlined. The relationships displayed in the mobile version and the same for the tablet and desktop versions.

Please click the below link to view the Figma file:

https://www.figma.com/file/Ef1YxeoB6ynW9VCMY6zRdx/T3A2?type=design&node-id=0%3A1&mode=design&t=bNSu0Xi3jqdfKIgB-1

# **R6**	
## Screenshots of your Trello board throughout the duration of the project

Due to some initial external challenges with successfully being assigned a partner, we first made contact with each other several days after our cohort's partners were assigned. Once we were assigned, we quickly gained contact on Discord, decided what project we would build and agreed to meet via a Discord call on the 31st of June. 

During the call, we created our Trello board and its tasks then assigned tasks to each other which gave us a good direction heading forward. We also created a repository on GitHub for Part A. After our first meeting, our Trello board looked like this:

![Trello-board-1](./docs/Trello-board-1.png)

During the process of working through the work required, we kept in frequent contact via Discord to kept each other updated. We shared this Readme.md document on GitHub and were able to both update it and use git pull requests to receive updates. 

After we had completed Part A, we had another call on Discord to coordinate the first tasks for part B where we decided to start working on the backend of the project. We then created a Trello Board for Part B and assigned each other tasks.

This is what our Part A Trello board looks like now:

![Trello-board-2](./docs/Trello-board-2.png)

Please click the below link to view the Trello Board:

https://trello.com/b/8YmuMz1R/t3a2-part-a

Please click the below link to view the Part A Repository:

https://github.com/Final-Full-Stack-Project-Team/T3A2-PartA
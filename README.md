# MERNproject-partA

Developers: **Jade Tyrer & Cassandra Zara**
Part A of final Coder Academy project - documentation for MERN app

## Outline 

#### Purpose
"Bespoke Nails" is known for creating unique and highly detailed hand-painted designs for nails, is based in the UK, and has an established instagram platform with a strong aesthetic and logo and a loyal customer base. Bespoke Nails (BN) functioned as an in-person apppointment beauty service prior to 2020, and with social distancing rules, has branched out to include pre-made stick-on nails that can be applied by the customer at home.   

The purpose of the application is to extend the online platform and functionality for "Bespoke Nails" to digitally manage customer appointments and orders more easily during the work from home era. The application should allow customer appointments and orders to be made online with a certain level of automation to circumvent all appointments being made via phone call or instagram direct messages which require a high level of time and effort to keep ordered. The application should allow the owner or admin to view and manage the calendar, see all orders in a central location, and send order confirmation and estimated pick-up time. The application should allow the customer to see availability and request an appointment, order pre-made stick-on nails or create a custom order for stick-on nails. 

Further releases of the application may see inclusion of customer authentication to see a history of appointments and designs for a more personalised experience and an online store to handle payments. 

#### Target Audience
Bespoke Nails has an established customer base in the physical location of the service, as well as a strong following on instagram engaging a younger generation through social media. The target audience consists of a younger cohort aged from roughly 14 - 40, with a strong interest in fashion trends, artistic expression and bright, bold design. Bespoke Nails attracts a large percentage of female-identifying persons though gender is not an exclusive characteristic of BN's customers. 

#### Features

##### MVP
The mimimum viable product has a scaled down number of features. The MVP functionality consists of authentication and authorization of an Admin user, CRUD operations for the list of items that can be ordered, as well as a form that the customer can use to create a custom order. The Admin is able to view the orders in the Admin dashboard and mark as completed which will in turn will affect the sorting of the orders. The application will also encompasss information about the brand including a menu-style display of appointment cost and options, such as a manicure, $35, 30 mins. For the MVP, the rendering of information including the 'About' and 'Portfolio' aspects will be static with the intention to develop with CRUD operations in a further release that can be utilized by the Admin to update the application themselves. 

In the MVP, the customer does not require authentication as customers have very limited authorization to perform actions. The customer is able to read and create an order, either by selecting a previously designed item or creating a custom order. The customer can view the 'About' and 'Portfolio' pages and complete a 'Contact' form for queries. 

##### 2nd Release

As visual imagery is a major component in selling the product, a prioritised feature during the 2nd Release is the use of the instagram developer API, so the admin can utilize the instagram feed in the portfolio section and streamline sharing of images of their work.

The second release extends customization of the order form, by giving customers the option to upload an image. Image storage is achieved through the use of Amazon S3 cloud storage. 

The second release incorporates calendar and appointment functionality. The visual calendar is accessed via the Admin dashboard once the Admin has been authenticated. The Admin also has the ability to perform CRUD operations on the appointments in the calendar manually, while the appointments made via the application by a customer are automatically added to the calendar. From a customer point of view, a customer can book an appointment by checking a certain day, with available time slots able to book via completion of a form with customer details and appointment options.  

##### 3rd Release

The third release of the application incorporates functionality for the customer to be authenticated and see their history of past appointments and orders. 

The efficiency of Admin-Customer communication is streamlined with the use of emails sent from the application to confirm the order and estimated time of completion for pick-up. 

The third release makes the Update and Delete CRUD actions available for the 'About' page to give the Admin more autonomy in managing the application as it renders (rather than uploading a PDF). 


#### Tech Stack 
The application is created using the MERN stack, which consistes of the following technology running in a Node environment: 

- A Mongo Database to manage data about appointments and customers (with appropriate authentication via passport in the server, and client). Documents for orders. 
- Mongoose 
- An Express Server which covers the back-end of the application 
- React to create the client application
- JavaScript libraries 
including calender _____, passport for authentication
- email service  
- Amazon S3 storage of uploaded images
- Deployment of the server with Heroku
- Deployment of the client with Netlify
- Axios as a HTTP client to manage request and response between the server and client
- instagram api

Project Management Tools
- Figma
- Trello
- Cardboard


## Architecture

## User Stories
Before Refinement:
![pre-refinement user stories](/images/original-US.png)

After refinement (MVP and prioritised release):
![refined user stories](/images/refined-US.png)

Admin User Stories
![Admin User stories](/images/refined-admin.png)

Customer User Stories
![Customer User stories](/images/refined-customer.png)

https://app.cardboardit.com/maps/134182

## Wireframes

## Dataflow diagram


Data Flow Diagram for MVP
![Data Flow diagram](/images/Data-Flow-Diagram.png)
Diagram Key (Yourdon & Coad conventions)
![Data Flow Diagram Key following Yourdon and Coad comventions](/images/dataflow-key.png)

2nd Release would include Calendar and Appointment features with CRUD operations. 

## Workflow

##### Methodology

The team will be following an agile approach to the project including using a Trello board to show task progress and completion as well as assigning tasks. 
This will follow a 'kanban' approach of continuous integration over the 4 week timeline with daily stand-ups to reflect on progress and workthrough problems. Following the Kanban approach there will be no required roles but rather shared responsibility and transparency where change can occur at any time rather than waiting for the end of a sprint (as in Scrum approaches). 

**Git**
A GitHub organization 'Zara-Tyrer' was created for the members of the team to support a shared workspace and repositories. 

3 repositories were created: 
- Part A: Documentation
- React client 
- Express Server 

Individuals then:
- Forked the repositories to individual accounts
- Cloned to local repository 
- Feature Branch is created
- Regular commits pushed to feature branch in forked repository
- Pull request is made to merge feature branch into central (original) respository

## Project Management - Trello Screenshots
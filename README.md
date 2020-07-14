# Bespoke Nails (MERN application): Part A

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
![pre-refinement user stories](/docs/original-US.png)

After refinement (MVP and prioritised release):
![refined user stories](/docs/refined-US.png)

Admin User Stories
![Admin User stories](/docs/refined-admin.png)

Customer User Stories
![Customer User stories](/docs/refined-customer.png)

https://app.cardboardit.com/maps/134182

## Wireframes

The design of the application has a consistent colour scheme to communicate the brand on every page. Pink, black and white are the predominant colours used throughout the application as they reference the Bespoke nails logo, and therefore the majority of the application (images will be refined based on accessibility testing at a later date) will adhere to contrast requirements that ensure accessibility. The colour scheme is designed to appeal to the target audience with the design encompassing a simple and modern aesthetic to appeal to a younger demographic and to further aid with the navigation between pages of the application. As the images used act as a portfolio that is evidence of the highly detailed artwork in each product, it was important that the surrounding content design was clean and simple to invoke the connotation of an art gallery setting and furthur elevate the product. There is minimal information displayed on each page to ensure the user is drawn to the key purpose and functionality of each page such as completing a form. There are descriptive links with clear navigation to pages with more specific information, for example, the about/prices page which is a key piece of information a consumer may want to know. This aspect of the design is aligned with the user stories and flow within the application.  
 
The navigation bar is consistently displayed at the top and bottom of every page when it is rendered to ensure the user can navigate quickly throughout the entire application amd familarity is quickly gained ensuring a smoother user experience. The landing page has a nail polish in the background to visually communicate the purpose and content of the application. There is a prominent order button designed to stand-out and direct the user to the shop, with the ultimate goal of the user ordering nails. This is strategically placed as the key feature on the homepage and clearly labelled so the user is aware of the action that clicking the button will invoke demonstrating content prioritisation. Colour and imagery is used to enhance space distribution to section the page and allow the user to note different features, for example purchase of gift cards compared to the lookbook where the user can see examples of the product. 

The secondary purpose of the site is for the administrator to track the products, orders and queries. This is accessed via the admin login at the bottom of the homepage, this link is displayed in the footer as it is not accessible to Bespoke Nail clients but is easily found for admin users that will be aware of where it is located. 

The admin user will be redirected to a dashboard upon successful login, that will display a summary of the queries and orders and will have side navigation that will display this information in more detail when clicked. Further releases will integrate the calendar and appointment functionality seen in the dashboard wireframe. The side navigation will also display a link to the shop which has a similar view to the customer but will also contain the extra links only the authorized admin can see and use to create, update and delete products displayed in the shop. The admin view will display the picture and username of the admin that is logged in with the logout button displayed below for ease of user control. 

There will be a completed message communicated to the user after they have submitted either order or query to ensure the user is aware that their requested action has been committed successfully. This message will include order details and/or details of what steps to expect next to ensure a quality user experience. 

![homepage](/docs/homepage.png)

When a user has entered their email to join the mailing list the option be will be greyed out as a visual indication the submission was successful. 
![submitted](/docs/submitted.png)

![admin-login](/docs/admin-login.png)

![dashboard-home](/docs/dashboard-home.png)
![dashboard-orders](/docs/dashboard-orders.png)
![dashboard-order-detail](/docs/dashboard-order-detail.png)

![order-form](/docs/order-form.png)
![order-complete](/docs/order-complete.png)

![about-page](/docs/about-page.png)

![query-form](/docs/query-form.png)
![query-complete](/docs/query-complete.png)

![user-shop](/docs/user-shop.png)
![lookbook](/docs/lookbook.png)

![admin-shop](/docs/admin-shop.png)
![create-product](/docs/create-product.png)

![giftcard-form](/docs/giftcard-form.png)

The prototype was designed using Figma demonstrating how the user can navigate through the site. The prototype can be accessed [here](https://www.figma.com/file/goZeDczPJzsj4Fe6HBzmLs/Wireframing-(Copy)?node-id=0%3A1). The link will open and the prototype view can be opened by clicking the play button ![play-button](/docs/play-button.png) in the top right corner. 

![prototype](/docs/prototype.png)  

##### Mobile Views

![mobile-homepage](/docs/mobile-homepage.png)
![burger-menu](/docs/burger-menu.png)

![mobile-dashboard](/docs/mobile-dashboard.png)
![mobile-order](/docs/mobile-order.png)
![mobile-about](/docs/mobile-about.png)
![mobile-query](/docs/mobile-query.png)



## Dataflow diagram

Data Flow Diagram for MVP
![Data Flow diagram](/docs/Data-Flow-Diagram.png)
Diagram Key (Yourdon & Coad conventions)
![Data Flow Diagram Key following Yourdon and Coad comventions](/docs/dataflow-key.png)

2nd Release would include Calendar and Appointment features with CRUD operations.

https://www.figma.com/file/ry0gd3MjyaOz7ZGgK0p8iz/Data-Flow---Bespoke-Nails-J%26C?node-id=0%3A1

## Workflow

##### Methodology

The team will be following an agile approach to the project including using a Trello board to show task progress and completion as well as assigning tasks. 

This will follow a 'Kanban' approach of continuous integration over the 4 week timeline with daily stand-ups to reflect on progress and workthrough problems. Following the Kanban approach there will be no required roles but rather shared responsibility and transparency where change can occur at any time rather than waiting for the end of a sprint (as in Scrum approaches). A Kanban board (Trello) was set up with the cards being moved between the 'To-do', 'In Progress' and 'Done' with user stories labelled by priority from 'MVP' and 'Beyond MVP', as well as 'Admin' and 'Customer' stories. Stories are also labelled to show complexity such as 'Authentication Not Required' to aid with time estimation. Prioritization of tasks will be determined in morning stand-up, loosely following building a feature with it's actions - such as customer order including viewing products in the shop, creating an order with the order form and receiving a confirmation message. Each card should take approximately 3 hours to implement but cards may be broken down further once the project starts after a few days if the expected timeframe is found to be inaccurate. Each card will be broken down into fitting out the backend logic, writing and running tests, integration and then front end in React.    

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

Trello was used to map out Part A. Requirements were added as well as important links and ideas. Requirements were allocated and tracked via coloured tag. 

![Trello Screenshot 1](/docs/Trello1.png)
![Trello Screenshot 2](/docs/Trello2.png)
![Trello Screenshot 3](/docs/Trello3.png)
![Trello Screenshot 4](/docs/Trello4.png)
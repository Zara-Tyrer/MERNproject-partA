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

**Admin**

- Calendar 
- Orders 
- Portfolio

**Customer**

- Make an appointment 
- Orders



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



## Architecture

## User Stories
https://app.cardboardit.com/maps/134182

## Wireframes

## Dataflow diagram

## Workflow

**Methodology**
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
# Projektseminar : WebApps for mobile Forensic Workshop

!Important: This repository is still under active development.

Within the project seminar two web apps were developed to provide students with a simple and modern way to test and check their knowledge. The lecturer app(Dozentenapp) is the part of the project seminar that is intended for professors and chairs. This web service allows the creation of questions and questionnaires divided into categories and subcategories. The student app offers the students the possibility to learn the questions and to test them realistically in an exam. The database is identical and is synchronized by a RestApi and a central MongoDB server. The idea of this project is based on two existing Web Apps, but these have been completely redesigned, since they only represent front-end applications without interfaces or a central dataset, which is absolutely necessary for the logical use of this project. The Forensic Workshop is hosted by the "TRIO Forschungsprojekt".

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

What things you need to install the software and how to install them

Install Node.js and a Code Editor by your Choise

### Installing

A step by step series of examples that tell you how to get a development env running:

So as you can see this Repository is splitted into 3 Submodules or child-repositorys:
- NodeJSServer
- Dozentenapp
- Studapp

# Cloning
1. Possibility:

Now we’ll clone this project with a submodules in it. When you clone such a project, by default you get the directories that contain submodules, but none of the files within them yet.
You must run two commands: git submodule init to initialize your local configuration file, and git submodule update to fetch all the data from that project and check out the appropriate commit listed in your superproject:

2. Possibility:

Use "git clone --recurse-submodules" to direct initialize and update each submodule.


Now when you have successfully cloned these projects:

All of these Projects use Node.js in one way or a other so you will have to install all needed node.js packages. To do so follow these steps:

1: Open up a Terminal and jump into a Project

2: Run "npm init -y"

3: Run "npm install"

4: For Dozentenapp and Studapp run "npm install chart.js"

5: For NodeJSServer run "npm i --save-dev nodemon"

6: For NodeJSServer create a .env File in the Repository. Of Course this File is normally not included into the repository.
   In this File create a new Variable with the connection String to your MongoDB Atlas cluster.
   Example:
   
  DATABASE_URL=mongodb+srv://brad:1234@projektseminar-oibte.mongodb.net/test?retryWrites=true&w=majority

## Running the tests

Once you installed all required Dependencies, you should start the "Dozentenapp" and the "Studapp" with a Live Server(extension for VSC) and test it.

To test the NodeJS Server open up a terminal and run : npm run devStart


## Deployment

To create an fully working Learning Environment System you should(of course) create and MongoDb Atlas Cluster and use the connection String in your .env File and host your NodeJSServer on a Server(We recommend Heroku)

## Built With

TailwindCSS
NodeJS
Mongoose
JavaScript
Express.js

## Contributed/Authors

Created by:
laefrost
robertbetschinger






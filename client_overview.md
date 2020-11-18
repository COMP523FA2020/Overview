---
title: "Client Overview"
permalink: /client_overview
---
[Home](/Overview/) |  [Project](/Overview/project) | [Team](/Overview/team) | [Journal](/Overview/journal) | [Deliverables](/Overview/deliverables) | [Client Overview](/Overview/client_overview)

## Overall Project Architecture

<img src="https://docs.google.com/drawings/d/e/2PACX-1vQ-fdJh91oJPH_JyRG85LArbDBjpiiCFDuYjytZ-0xZuUt9afiJ_MpOJVJm-emyyuwfSvCmFejkP-Z1/pub?w=960&amp;h=720">

### Major Components

#### React Frontend

The frontend is built using React. It contains a root component called App defined in the App.tsx file. This component is rendered in the root HTML file, index.html.

TODO

#### GraphQL Backend

**Simple**

The backend is a server with connection to a MySQL database that exposes a single endpoint (e.g. [http://back-end-dept-dietdatabase.cloudapps.unc.edu/graphql](http://back-end-dept-dietdatabase.cloudapps.unc.edu/graphql)) where clients (e.g. the frontend) can send a request and get the data it needs. The backend will then query the MySQL database and return the data in a specified format back to the client.

**More Detail**

The backend is an Apollo GraphQL server that exposes a single endpoint where clients can send a request in the format specified by the GraphQL query language. The request specifies a specific query the backend makes available and passes in any necessary variables. After receiving the GraphQL query from the client, the backend will then resolve that query using resolver functions (located within the Resolvers directory) that corresponds to the specific GraphQL query. Within the resolvers, the backend uses TypeORM to send the appropriate SQL queries to the MySQL database, which will return the requested data. The resolver will then reformat the data as necessary and return the data, which is then sent back as a response to the requesting client.

The GraphQL schema (read more [here](https://graphql.org/learn/schema/)), available queries, as well as examples of requests and returns are located in [this Google Doc](https://docs.google.com/document/d/1AFhOHjLNl7l94i2NTPFfHFaCq1IXeK4Lfre-KeErWWY/edit?usp=sharing)

#### MySQL database

The database currently contains three tables
1. avian_diet
- Where all the main data is stored. Data is from [this](https://github.com/hurlbertlab/dietdatabase/blob/master/AvianDietDatabase.txt) .txt file with the same column set up as described in the .txt header row.
2. table_history
- This table keeps track of the last time a specific table has been updated. It contains two columns, "table_name" and "last_updated". Currently this table only contains information for "avian_diet". The "last_updated" column of the "avian_diet" table is updated every time the "avian_diet" table is updated. More info under the "Python Script" section below.
3. regions
- This table contains a single column "region_name" that are valid regions that users can filter the "avian_diet" table with.

The TypeORM entities within the backend (located at src/entities in the project directory) species what tables will be created and interacted with.

#### Python Script (not in diagram)

Apart from the above three components, we also have a Python script that does the job of updating teh table using data from the github .txt file linked above. If the last commit to that file was made less than 7 days ago, the script will:
1. Create a new table in the database named "avian_diet_new"
2. Adds the new data from the .txt to the table
3. Renames the current "avian_diet" to "avian_diet_old" (deleting previous "avian_diet_old" if exists)
4. Renames "avian_diet_new" to "avian_diet"
5. Updates record in "table_history" table with the "avian_diet" table name with the current timestamp

This means that the previous avian_diet table will be stored under avian_diet_old

#### Carolina Cloud Apps

Each of the above components are deployed/run on this platform. The Frontend, Backend, and MySQL database are deployed as applications within the project (client has knowledge of what this project is) and the Python script is a cron job scheduled to run every Sunday @ 00:00:00 UTC within the platform.

## Client Access to Project

In order to manage the project, access to the Carolina Cloud Apps project is necessary, which our client (Professor Hurlbert) already has. Here, one may shutdown services, add new applications, change the cron job scheduling, and etc.

## Features

### Need-To-Have

In the beginning of the semester, we went over the necessary features as well as features that were nice to have. Here is an update on that checklist!

[Complete] Web users are able to store the query results by downloading data from the results table.
- After the user queries on a specific bird or prey, he can download the tbale as a CSV file.

[Complete] Able to query the database using different criteria such as seasons, year range, and region.
- The user can change the criteria using the dropdowns on the result page. The table as well as the map and graphs are updated dynamically depending on the filters.

[Complete] Able to see an overview of the avian data by using bar graphs that categorizes the different studies.
- On the predator page, there are three bar graphs: records per season, records per decade, and records per diet type.

[Complete] The result page updates dynamically as users update the criteria
- Table, graphs, and map all dynamically update depending on criteria

[Complete] Users can query for data based on predator or prey.
- There are two search bars on the hompage, one for predator and the other for prey. There are two results page for predator and prey.

[Complete] Users can navigate between predator and prey by clicking on their names in the results table.
- Each name on the results table is hyperlinked to the respective page

[Incomplete] Users can share query results by using the URL.
- Currently the URL of the website is static even if search and criteria changes.

### Nice-To-Have

[Complete] Search bar has autocomplete as the user is typing in the name of a bird or prey.
- As users type the scientific or common name of a bird or prey, the serach bar will autocomplete and give up to 10 results that contain the typed text

### Highest Priority Next Step

The highest priority next step is to add dynamic URLs. The URL should change depending on the item that the web user is looking up. Furthermore, even for the same bird, the URL should vary depending on the specific criteria choices. With this added feature, web users can share specific query results and interesting findings.

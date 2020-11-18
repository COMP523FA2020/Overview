---
title: "Deliverables"
permalink: /deliverables
---
[Home](/Overview/) | [Project](/Overview/project) | [Team](/Overview/team) | [Journal](/Overview/journal) | [Deliverables](/Overview/deliverables) | [Client Overview](/Overview/client_overview)

### Assignment 1: Trello Board
- [https://trello.com/c/W9sxRC4J/3-assgn2-web-site](https://trello.com/c/W9sxRC4J/3-assgn2-web-site) (private)

### Assignment 3: User Stories
- [Under Project Section](/Overview/project)

### Assignment 4: Clickable Prototype
- [InVision Project](https://projects.invisionapp.com/prototype/BirdyDesign-ckf4o3rnp0013tx01kkjjzjlc/play/60539f25)

### Assignment 5: Apples Reflection 1 (Click on name to dropdown)
<details>
<summary>Muyan's Reflection</summary>
One goal of the Avian Database Project is to aggregate all information related to a bird’s diet. The project offers users the flexibility to query the data with varying criteria. The first target audience of this project are scientists or researchers who wish to gather that information. For example, if a researcher wants to know how a specific bird’s diet will change from season to season, he is able to use the website’s filters to find out. This website can become the central place that researchers can go to when trying to query the diet database of birds.

To help researchers access the appropriate data, we will implement many different filters and criteria that will affect their results. The user can modify the results by region, season, time, and species categories. Furthermore, there are graphs near the query results that summarizes the main information. Those graphs can help the researcher visually understand the data trends better and can also be a tool that the researchers could use in their future presentations.

Another target audience for this project are the general public who are curious about bird diets and wish to explore more. The website can bring more public interest to wildlife and the environment. Currently, there lacks a concentrate database where any individual can look up what different birds eat, so this project fulfills that need. We hope to make this website new-user friendly by having different query options. If the user already has a bird in mind, he can type in the bird to learn about its diet. However, if the user doesn’t have a particular bird that he wants to look up, he can also query the database by prey. Another aspect that promotes new-user friendliness is the autocomplete option in the search bar. A person visiting the website can start typing in any bird’s name, and the autocomplete will suggest a whole array of options for the user to explore
</details>

<details>
<summary>Teddy's Reflection</summary>
The project that I have been developing with my group is a bird diet database. Prior to the creation of this database, there has never been an accumulation of this data on this scale before. In said database, there are archived studies (tracing back decades). Our app will provide researchers with access to this data in a user-friendly way. From this data, researchers might find insights into how bird’s diets have changed over the years. From the categorization of this data, there may be inferences that can be made about the effects that climate change, habitat destruction, and human industrialization/development have had on the health of ecosystems around North America.
</details>

<details>
<summary>Thomas's Reflection</summary>
Our team on the Avian Diet Database project aims to fulfill Professor Hurlbert’s need of allowing common internet users access to his team’s database of avian diets. This database is a collective of information from many different sources compiled by Hurlbert, his team, and other contributors. Since this is a compilation from many different sources, the information it contains is vast and could be extremely helpful for scientist observing trends relating to avian diet over the years. However, it requires technical knowledge in R programming to be able to query information from the data. We fulfil the need of allowing untechnical users access to the database by providing a website with a search bar that gives users ability to search through the database in a similar manner as common search sites (e.g. Google, Bing, etc). Aside from giving everyone easy access to the database, Professor Hurlbert plans on publishing a paper relating to his database. The site would give readers of his paper or those interested and easy way to look at the work he has done.
</details>

### Assignment 6: Application Architecture

#### React

**Summary**

In order to quickly create a complex and interactive web app, we decided to use the React framework.

**Problem**

Our client wants users to have a real time experience, where data transforms as they manipulate parameters. Web frameworks are a necessity for creating these kinds of experiences

**Constraints**

None

**Options**

Vue
- Pros: Simple syntax and learning curve, smaller in size (comparatively)
- Cons: Smaller than Angular or React, maintained by small group

Angular
- Pros: Good typescript support
- Cons: Little harder to learn (comparatively)

React
- Pros: Frontend team already knows react
- Cons: Not as featured as Angular.

**Rationale**

Since two group members already had experience with React, we decided to stick to it in order to avoid a learning curve with a new framework.

#### GraphQL

**Summary**

In order to create an organized API that works well with complex queries, we decided to use GraphQL.

**Problem**
The nature of the app requires querying a backend database with 5 or more potential parameters on any given query.

**Constraints**

None

**Options**

Rest API
- Pros: More common, other people may have an easier time integrating their own systems with our backend.
- Cons: As the queries rise in complexity, the request URLs may become unmanageable.

GraphQL
- Pro: Simplifies complex queries and return types.
- Con: More of a learning curve, potentially more trouble to set up in the backend.

**Rationale**

A REST API for this solution would look incredibly clunky: but given GraphQL's query and variable system, a clean solution is much easier. The simplicity gained outweighs the cost of initially learning it.

#### Bulma
  
**Summary**

In order to style our web page, we decided to use Bulma as our CSS framework.

**Problem**

We want our website design to be responsive on different platforms. If the user decides to view our project on their mobile device instead of their computer, our site can adjust responsively. In addition, we want the designs on our website to be familiar to the users. This is important because they can navigate through the site easier and it's more intuitive.

**Constraints** 

None

**Options**

Plain CSS:
- Pro: we have more options when styling our website, we aren't restricted as much
- Con: no built-in library that we can use (css made for a button), might not be responsive on different devices

Bootstrap:
- Pro: intuitive class names, large library of different UI components
- Con: many pre-defined styles so the users don't have a lot of choice, repetitive (dull) styles

Foundation:
- Pro: more flexibility when compared to Bootstrap, neat features like form-validation
- Con: Small community (less forum responses), more freedom so users might be overwhelmed by the list of options

Bulma:
- Pro: good documentation, easy class names, designs are responsive on different devices, good range of styles
- Con: built-in classes so users have less freedom, less components when compared to Bootstrap

**Rationale**

We decided to use Bulma as our CSS framework because Bulma has intuitive class names that make CSS styling easy. Bulma also has a limited amount of design components, so we can play around with different styles while avoid being overwhelmed. Bulma keeps up-to-date documentations on their service, which makes it easier to troubleshoot. Lastly, Bulma is responsive on difference devices and can adapt to different platforms.

#### TypeScript
  
**Summary**

In order to use a programming language that defines different variable types, we decided to use TypeScript.

**Problem**

When a language doesn't define a specific type for its variables, it might be confusing for the user to know the exact state of that variable. It can be difficult to debug without knowing the type and state of an variable. 

**Constraints**

We want to use a frontend-focused language that all of us have had experience with, so we are comfortable from the beginning.

**Options**

JavaScript
- Pros: simple, popular so more documentation, client-side so less work is put on the servers
- Cons: types aren't defined so bugs are discovered at run time, different browsers will interpret code differently

TypeScript
- Pros: types are defined, additional features like interfaces and generics that don't exist in JavaScript, compile time type checking
- Cons: longer code when compared to JavaScript that might not add any clarity

**Rationale**

We chose TypeScript over JavaScript as our frontend language because we want to have our types clearly defined. Bugs will be discovered earlier at compile time rather than at run time. Also, the users will know the exact state of a variable rather than inferring it. 

#### MySQL

**Summary**
In order to access the data provided by Prof. Hurlbert and his team in an efficient, reliable, and standardized way, we decided to use MySQL.

**Problem**

The backbone of the Avian Diet Database project a database that is currently  a tab deliminated text file. Prof. Hurlbert's current method of querying is a set of R functions that he wrote himself. This is hard to integrate cleanly with our chosen backend technology (GraphQL).

**Constraints**
Client prefers MySQL

**Options**

Flat Text File
- Pros: No need to use DBMS, no need to transform data to migrate to database (can reuse client logic in R functions)
- Cons: Have to parse file ourselves, still have to transform data to work with backend

A DBMS
- In terms of DBMS, any of the popular ones would work fine. The database is relatively flat and small so there is no huge benefit between them.
- Pros: Reliable, easily accessible, scalable
- Cons: Have to transfer current .txt format to a DBMS

**Rationale**

Since we decided to use GraphQL as the API to serve our data to the frontend, we can easily fit this with the data by using TypeORM with a database like MySQL.
Furthermore, using SQL to query the database rather than creating our own parser for a text file would be much more efficient in term of time and manpower.
We ultimately chose based on client preference.

#### Carolina Cloud Apps

**Summary**

In order for the frontend to access our APIs, we decided to use Carolina Cloud Apps to host the backend and database.

**Constraints**

Client prefers Carolina Cloud Apps

Database has 50,000+ records

Free is preferable

**Options**

Heroku
- Pros: Learned how to use in class, a lot of easily accessible documentation, straightforward to use.
- Cons: Free tier has limitation on memory.

Carolina Cloud Apps
- Pros: University supported so can get direct help from team running service, able to increase memory limit for free
- Cons: Documentation is a little hard to find, a bit more complicated to set up than other services, requires connection to UNC VPN

**Rationale**

Since the database contains over 50,000+ rows, it exceeds the free tier limit that Heroku provides. This is a similar issue for other services.
We decided to use Carolina Cloud Apps because Prof. Hurlbert is able to increase memory limits for the servers for free if needed.
Having the backend also in Carolina Cloud App allows easy interaction between it and the database.
Furthermore, client prefers Carolina Cloud App, since he is able to get direct assistance with University staff if any trouble is to occur.

### Assignment 7: Application Diagram

<img src="https://docs.google.com/drawings/d/e/2PACX-1vQ-fdJh91oJPH_JyRG85LArbDBjpiiCFDuYjytZ-0xZuUt9afiJ_MpOJVJm-emyyuwfSvCmFejkP-Z1/pub?w=960&amp;h=720">

### Assignment 8: Walking Skeleton

[http://frontend-dept-dietdatabase.cloudapps.unc.edu/](http://frontend-dept-dietdatabase.cloudapps.unc.edu/) (Link subject to change)

### Assignment 11: Test Coverage Report

### Backend Coverage Report

<img src="https://drive.google.com/uc?export=view&id=1ieI89PCZnHACfql7mUvyiFb9Bn3PWfM8">

This is the test coverage report for the backend of the AvianDietDatabase project, specifically any utility functions and GraphQL query resolvers. The testing framework we use is Jest.

**Test Suite Health**

If we are going by *overall* health of the test suite, I do not believe looking at test coverage can really determine anything substantial about a test suite since quality of test matters more. At most, if coverage is high, it indicates we at least have tests that cover most of our code, which *might* be better than nothing.

If we are just using coverage as the measure for health, I woulds say that the report indicates a "healthy" test suite, given that it covers most of the lines of code, at 91.44% coverage.

**Parts Not Tested**

One part of the code we don't test is the `AvianDiet.ts` file, which contains our AvianDiet entity. It is not directly tested against because we indirectly test it when we test our resolvers, which operate with the object. We expect certain fields from the AvianDiet entity when using our resolvers, and if our resolver fails, we can pinpoint the error being related to our entity if needed. Also AvianDiet entity does not contain any functions that we write where we expect certain return values, it is just a class with certain fields. The test coverage report indicates that 0% of functions under `src/entities` (our `AvianDiet.ts`) are covered. This is because we includes two lambda functions within our @Field decorators to indicate that this TypeGraphQL field is an Int. This is related to generating a GraphQL schema, so it would be odd to test the lambda functions in the decorator.

We don't test any files under `src/migrations` since those are generated files from our AvianDiet entity.

Finally, we don't test any files under `src/tst/tst-utils` since those are used for our testing and simply sets up a mock database and TypeORM connection. It is marked as "covered" in the report since we use those functions in our testing.

**Top Priority**

The top priority in testing would be the resolver functions, as the values they return are the values received by clients who query our backend server (in our case the client is our frontend website). These resolvers are essential since they would be providing the data that the whole project revolves around.

**Unsure How to Test**

I feel that `index.js` is important to test since this is where the express app and ApolloServer are created/started. The expected functionality is to start up successfully, so I wasn’t sure how to tackle testing. What I’ve looked into is integration testing by mocking an ApolloClient (provided by apollographql), and starting up a test ApolloServer, similarly to how I set up a test database. However, most examples I’ve seen, it seems to be a separate Integration Test file rather than directly using index.js.

### Frontend Coverage Report

<img src="https://drive.google.com/uc?export=view&id=1TVkm_wtloqKAVxXYW-eV3YJpBTQwrdvy">

<img src="https://drive.google.com/uc?export=view&id=1-ZK57JNnVsFVWU9MPrQNZXJyUzxZPIdl">

<img src="https://drive.google.com/uc?export=view&id=1TRBB1QRUFZuorVfIb7IEHwHMVD4llqUG">

We used Jest to test our frontend code. 

**Test Suite Health**

The results of our tests represent a semi-healthy test suite. We were able to cover the most important frontend features like the query table, but we were unable to cover some files like the search bar. We are comfortable with this outcome. 

**Parts Not Tested**

With features like the search bar, we are just sending an API call, so most of the logic is done in the backend. In our frontend testing, we want to focus on features where a lot of the logic is put on the frontend like sorting within the table or creating the states map. 

**Top Priority**

The top testing priority is the query table on the item page. That table contains the data that researchers or everyday visitors can use or read. A huge challenge when creating the table was ensuring that our web visitors had the flexibility to sort and modify the table using many different criteria. This motivated us to write many sort tests to make sure that moving around data in the table or modifying the data won’t produce any bugs. Sorting is a feature that almost all of our visitors will use, so we want to cover all of the use cases. 

**Unsure How to Test**

Another important feature on the frontend is the graph section. We weren’t sure of how to test that feature. The logic of retrieving the correct numbers comes from the backend, so on the frontend, we are only trying to visualize that data. In the future, more time can be spent on making sure that the graph is formatted correctly for the client

### Assignment 12: Developer README.md
[Frontend Repo](https://github.com/COMP523FA2020/Frontend)

[Backend Repo](https://github.com/COMP523FA2020/Backend)

### Assignment 14: APPLES Reflection 2

#### Muyan

My impression on my client’s purpose has remained the same. Avian Diet Database has two main goals. One, this website allows researchers or students to query through the backend database. If a researcher wants to know exactly what certain birds eat during a specific season, he can make that query intuitively using our website. This project gives researchers the ability to modify their queries. The second purpose of this website is to introduce birds and their diet to everyday individuals. If a child wants to look up a random bird and learn what it eats, he can do that easier through the homepage.  

I am more excited about the website’s goal of introducing birds and their diet to everyday individuals. While the graphs and map that summarize the query results are informational, they are also fun and can attract an audience. These visual aids can help give an overview of the query results, so individuals don’t have to scan the query table row by row. The website also caters to both researchers and everyday folks by allowing individuals to look up a bird by its common name or scientific name. This feature allows everyone to look up the bird that they are interested in! 

Our project does not add any new information about birds and their diet. The information is already there; we simply created a website that allowed individuals to query that information. However, instead of running complex scripts to look up specific diet information, our users can now select a few dropdowns, and the information will be returned to them both in a table and in various visual representations. Our website will cut down the time that researchers use to find useful information. More importantly, no individual is going to become interested in birds and what they eat through a database; they would only be overwhelmed. Our website provides them an opportunity to look at birds that interest them and returns that information in a fun style.

#### Thomas

My impression up until now of our client’s purpose and clientele is still the same as it was back when we first started. Our client, Professor Hurlbert has been clear in defining who the audience of this project would be and why he wants this project to exist. To reiterate, the audience of our project can range from casual users wanting to check out the website and its bird database, to researchers and scientists who are looking for specific data or to find trends. As for the mission/purpose, it is still to provide those users with a clean and easy way to search through the data Prof. Hurlbert and his team collects. We are able to maintain this understanding do to our weekly meetings, and so far it has not changed.

I have been, and still am, excited about this mission ever since I saw the client presentation. I find it admirable that Professor Hurlbert and his team wants to create a way to share the information they have in an accessible manner. This spread of information is what makes the Internet so great to me, and it is exciting to be able to participate. Furthermore, I see this project as more than the usual projects I create that gather dust on GitHub.

The product our team is creating, the Avian Diet Database website, helps accomplish this mission by providing a nice website with search bars that allow anyone to look up birds and their prey by name. This type of site closely resembles other familiar search sites such as Google or Bing and is intuitive to use. After looking up a bird or its prey, users are also presented with the data in a table that is easy to read as well as several graphs on the side to help visualize some of the data. All of these features combined together makes it so that users can easily access information on the database.

As for some of the most important features, one would be the core components of the frontend. There would be no functional website if these did not exist. This includes the two search bars we have in the homepage (one for Birds and another for their prey). The seemingly simplistic style is intuitive for most users, which in turn helps the mission of allowing a variety of different users to look through the database. Another is the results page that shows a table of the results, as well as graphs to help visualize. This is the data our client wants to present to users. Furthermore, we have filtering capabilities (e.g. filter by season, year ranges, etc.) that are important to our client. The other set of important features would be in the backend that provides the information for the frontend. These are the GraphQL queries that the frontend uses to grab the data and display them. By storing Professor Hurlbert and his team’s data in a database and serving it to the frontend, it helps in allowing users to look through the database. Overall, the backend allows access the data and provides an easy way to serve data to the frontend, and the frontend gives users a clean UI to look through the database.

#### Teddy

My impression of their purpose has not changed very much. The goal has remained to provide intuitive access to the wealth of information accumulated by Professor Hurlbert’s team. Approaching a final product has made me significantly more excited about the mission - being able to see the impact of my work on a real-world problem is a very valuable experience. Our product allows researchers to query the bird diet data in very specific ways, facilitating the exploration of complex research questions with real-world applications. With our product, it is possible to track changes in bird’s diets over time, the prevalence of both birds and their prey in areas over time, and using data like this it is possible to interpret some ecological trends. These are important to help preserve wildlife that may be impacted by climate change or human intervention.

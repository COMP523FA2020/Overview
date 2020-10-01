---
title: "Journal"
permalink: /journal/
---
[Home](/Overview/) |  [Project](/Overview/project) | [Team](/Overview/team) | [Journal](/Overview/journal) | [Deliverables](/Overview/deliverables)

## Meeting Schedules

### Client
- Fridays at 3pm

### Mentor
- Wednesdays at 4pm

### Team
- Mondays at 4pm

# Journals

**Caronlina Cloud App Meeting 9/29**

**Overall Picture: Kubernetes and Docker images**

How the platform works is that it adds our code on top of an image (e.g. openshift/node.js image) and uses docker to build a new “golden image”. This is what will be used to deploy.
For the most part, deployments are stateless. If we redeploy, changes on the running pod will be gone. However, we can get persistent storage by setting up application with a storage volume.

-	Won’t go into too much detail about this unless necessary
In terms of possible memory limitations:
-	The dept-dietdatabase project has increased resources compared to our personal projects.
-	We can request increase on resources with justification (e.g. out of memory when building app)

**Other Important Points**

-	For a NodeJS project, the default way it will be deployed is with a “start” script in package.json if applicable. We can modify this by setting the NPM-RUN env variable. For more details https://github.com/sclorg/s2i-nodejs-container/tree/master/10 
-	The dept-dietdatabase project will not go idle like personal projects do
-	If you try setting up your own personal projects on Carolina Cloud Apps, you will notice deployments will go idle after a while. This is not the same for dept projects, so we don’t have to worry about that.
-	Probably avoid trying to build our own docker image, some security concerns.
-	Don’t put passwords/any important information in the actual code base. Use environmental variables.
-	If we need any additional help, email cloudapps@unc.edu
-	https://help.unc.edu/sp?id=search&t=kb&q=cloudapps has documentation, but might be a bit tricky to look through.
-	As for running dev deployments, we can either do this in the same projects with different built applications for dev vs prod. Completely up to us/Hurlbert.
-	If we need help running our application on the platform, we can contact them for a 30 min session of sorts.

**Birdy Meeting 9/28:**

**Architecture diagram + system**

- Divided up the decision write up:
- Thomas: MySQL, Carolina Cloud Apps
- Teddy: GraphQL, React
- Muyan: TypeScript, Bulma
- For the diagram, Teddy added names under the logos and included more information like tools and languages

**Walking Skeleton**

- Each member gave an update on what they are working on
- Hoping to show Jacob an update on Wednesday

**Client Meeting 9/25:**

**About Database**

-	If we are able to, with respect to storage limits, Hurlbert would prefer to include all information in the MySQL database, in case they get used in the future. Happy to cut down on some data if necessary.
-	In regards to the map and data points that aren't strictly states (i.e. Southwestern US), would be nice to have a summary of those data points next to map and disregard adding them to the count for each state.
-	In terms of searching birds, good if user can provide both common name and scientific name, and still have autocomplete.
-	In terms of searching prey, not enough data on common name, so would have to search by the different taxonomic level. E.g. users can search at any level and receive results.

**Next steps**

-	Our group will keep working on the walking skeleton
-	Meeting with Thomas next week to learn more about Carolina Cloud Apps (didn't get to last week)

**Mentor Meeting 9/25:**

**Recap of Meeting with Professor Hurlbert**

-	Professor Hurlbert thought that having two search bars is more informational
-	We should document all of the interactions and choices that are made during meetings
-	Informative to look back on our notes to see why we decided on some choice

**APPLES Reflection**

-	Looks good; updated on our website

**Architecture Diagram**

-	The best diagrams are the ones where a developer and look at it and understand the situation well enough to start coding
-	Review some of the diagrams that Jacob have sent to us; implement the idea of swim lanes
-	There are online diagram builders that we can use to map out our architecture
-	Really emphasize the relationship between components and how they will affect each other

**Action items**

-	Small changes are still needed on the architecture diagram (we need to talk about some API calls)
-	Continue working on the walking skeleton; will demo that to Jacob this Wednesday
-	Thomas will meet with Professor Hurlbert to talk more about databases

**Birdy Meeting 9/21:**

**Recap**

-	Teddy and Muyan are focusing on creating the front-end with React
-	Thomas is looking more into the database + Carolina Cloud Apps
-	Regarding the homepage, the components will include an “about” button, 2 search bars, texts, bird image
-	More information about the project will be at the bottom of the homepage; button will take you there

**Plans for Wednesday**

-	Update Jacob on what happened with 2 vs 1 search bar
-	Will not show him the clickable prototype
-	Compare prepared with any questions that we want to ask

**Future plans**

-	We will host the back-end on Heroku and the front-end on Carolina Cloud Apps
-	Heroku free will only allow 10,000 lines for the database, so that might be the problem
-	Thomas will meet with Professor Hurlbert on Friday to talk more about database
-	Code session on Friday
- Email Thomas with Apples Refection, so he can update it on the website

**Client Meeting 9/18:**

**Giving Professor Hurlbert Updates**

-	Still going to keep improving on the design, but we feel like it is in a good place right now
-	We are getting started on the walking skeleton, so we can see how the design looks on an website
-	We would like to schedule a meeting to learn more about Carolina Cloud Apps

**Design feedback**

-	Professor Hurlbert still prefers two search bars over one
-	Having two search bars with the context sentence really helps the user understand what he is doing
-	Much easier and intuitive foe new users
-	The button to flip from predator to prey needs to be more clear
-	The results table can range in size, so we have to think about handling that
-	The results can appear before the graphs/states map

**Next steps**

-	Our group will keep working on the walking skeleton
-	Meeting with Thomas next week to learn more about Carolina Cloud Apps

**Mentor Meeting (9/16):**

**Design**

-	Even the perfect user needs a clickable prototype
-	Make the criteria much more clear; the user might not know that they need to change the criteria
-	Replace the underlines with appropriate icons so that they attract the users
-	The current design uses too much underlines, so that might need to be changed
-	Jacob agrees with Teddy’s search bar design, so we will incorporate that into the clickable prototype
-	Use 5 why’s to question Professor Hurlbert on the search bar
-	Get some users and have them decide on which search bar looks better

**Future notes**

-	Anytime that we make a change to the walking skeleton, have Professor Hurlbert look at it and get some feedbacks; make sure to record those feedbacks
-	We might forget some details so recordings are useful
-	Don’t just record what they say but also their actions (how their mouse cursor is moving)
-	Feedbacks are useful when we prepare for our final presentation



**Birdy Weekly Meeting 9/14:**

**Recap**

-	Continue working on the design (implementing 2nd round feedbacks from Professor Hurlbert)
-	Muyan and Thomas will watch the resources videos that Teddy provided
-	Thomas set up Carolina Cloud App and played around with it

**Action items**

-	Continue looking at different data schemas and how to convert the text files data formats that we can use
-	Sync up on how the front and back ends will communicate
-	Update design with features that both Muyan and Thomas created


**Client Meeting 9/11:**

**User stories:**

-	Teddy went over the user stories with Professor Hurlbert; everything is good there

**Design:**

-	Professor Hurlbert wants the search bars to appear on the homepage by default (without any clicks)
-	Prefers 2 search bars over 1
-	Professor Hurlbert likes how the description is included on the homepage; he will provide us a text for it
-	Get rid of the “prey level” graph, and put the states map into the 2x2
-	Number of records and studies should be more visible
-	Nice to have: studies will be hyperlinked to a popup that shows the actual studies
-	In the filter box, make the criteria flow within a sentence (keep the check boxes though)
-	Data sources are at the bottom of the page, and they should change based on the filter
-	No navigation bar
-	Change to the description font to match the title font

**Questions:**

-	Open to exploring other databases, but prefers MySql based on familiarity and ease
-	Thomas showed another design to Professor Hurlbert which he liked; will incorporate both design features into the final design


**Mentor Meeting (9/10):**

**Talked about meeting with Professor Hurlbert:**

-	Better to received feedback early on in the process
-	Now we know what Professor Hurlbert is expecting, so we can start modifying our project

**Went over the user stories:**

-	Overall, the user stories captured the features well
-	Fixed some wording and grammar issues
-	We should add an out-of-scope category to our user stories
-	They are meant for features that aren’t expected this semester like the user being able to modify the Avian Database
-	Good to have those stories on paper, so there aren’t confusion between us and Professor Hurlbert on what is expected

**Design:**

-	Jacob sent us a link to HackerNews about design tips; definitely take a look at it; link is in Slack
-	With the bar graphs, decide which ones the user would prefer to see first
-	With the states map, we can have dots representing the different studies being done in a specific area, and when we zoom out, we would get a number telling us the total number of studies (nice-to-have function)
-	On the homepage, it is not useful to have all those different statistics; maybe just have a search bar on the homepage where the user can look up both birds and prey
-	The above feature might bring up some issues when trying to access the database
-	Professor Hurlbert had change his mind after seeing the design, so we should be flexible

**Architecture:**

-	Our architecture drawing looks good right now
-	Jacob sent us some more examples in Slack that we can take a look at 


**Weekly Group Meeting (9/7):**

**User Stories:**

-	Went over user stories on Trello board, decided as a group if there are any more user stories that we wanted to add
-	Added two more stories to the “nice-to-have” column
-	Teddy will send our user stories to Jacob on Slack so he can look over them and provide feedbacks before Wednesday

**Design:**

-	Going to implement some changes to our design based on feedback from Professor Hurlbert
-	Going to show Jacob our design on Wednesday for additional feedback
-	Make a copy of the design to include in our presentation later on (changes over time)
-	Teddy and Muyan will continue working on the design this week

**Backend:*

-	Teddy has posted some useful video about API and backend stuff, so Muyan and Thomas should take a look at them when possible
-	We still have some questions when it comes to using Carolina Cloud Apps
-	Teddy recommended some videos 
o	https://www.youtube.com/watch?v=7giZGFDGnkc&list=PL55RiY5tL51rG1x02Yyj93iypUuHYXcB_
o	https://www.youtube.com/watch?v=65a5QQ3ZR2g&list=PL55RiY5tL51oGJorjEgl6NVeDbx_fO5jR
-	Decided to use MongoDB
-	Muyan will send Professor Hurlbert an list of onyens for Carolina Cloud Apps
-	Ask Jacob if Carolina Cloud Apps is actually needed on Wednesday
-	For feature code changes, we should have a blueprint before we start coding that needs to be approved (along with a Code Review at the end)

**Client Meeting (9/4)**

**Professor Hurlbert’s feedback on the design:**

-	Prefers a specific URL with each bird/query; easier to share the results with others
-	Get rid of 2nd page of the design; we can put the search bar on the home page to minimize clicks
-	Get rid of the random species feature
-	Prefers to have all 4 graphs displayed at once; 2X2 grid
-	Graphs should have fixed width? (have to brainstorm how the graphs would look on different monitor sizes)
-	Data sources should be at the bottom of the page; the table results should be at the center of the page under query criteria 
-	Don’t make bird 3 on the query page a dropdown 
-	Think about having dynamic pages, so we don’t have to use a refresh button
-	“data from” summary should be moved to the left of the page
-	Check boxes should be under the summary and before the results table
-	Make sure that the user knows that the check boxes will impact the results table
-	Modifying the checkboxes will affect the url?
-	Include a description on the home page
-	Get rid of the brown color (and the leaves); Professor Hurlbert will provide us with a theme
-	Add a navigation bar at the top of every page

**Mentor Meeting 9/2:**

**Jacob going over the website:**

-	Website is looking good; being updated frequently
-	Jacob went through the different requirements for the website making sure that they are present
-	Jacob had trouble accessing the summary and description LOL

**User stories:**

-	User stories can either take 5 minutes or days; really depends on how much thought we put into them and well we are communicating with Professor Hurlbert
-	Don’t be afraid to write additional user stories; those can help us be more aligned with Professor Hurlbert’s vision, and we can always drop them if we don’t finish like they are needed in the future
-	User stories can be really useful since they act as a constant reminder of what we need to do
-	User stories really shouldn’t be specific at all; think about the large goals that the user is trying to get out of our web application
-	Create a user story even if we aren’t ready for it; can always put it in the backlog

**Git collaboration:**

-	We all have different roles, so we should communicate our needs with on another
-	Before code reviews, just have a meeting where we show each other our code and what they accomplish
-	Things that we share and stress about in our code reviews should be different than the things we share with Professor Hurlbert (different level of details)
-	Swim lanes and web sequences can be useful to show our expectations of one another
-	Make sure that our solution can be useful from start to finish

**Communication notes:**

-	We should be constantly reviewing our meeting notes with Professor Hurlbert when working on design and coding
-	When Muyan is working on the design, he should go over it with Teddy and Thomas so ensure that everyone’s thoughts align
-	There are pros and cons for choosing different technologies, so we need to talk it over together
-	Every day of the week should have a different purpose and schedule
-	The design always has to stay ahead of the development team, however, we can start thinking about backend calls when working on the design
-	Others can work on the code even if Muyan isn’t complete with the design
-	Get some parts of the design into code so we can have something to show Professor Hurlbert
-	Hurlbert won’t get his peers for reflections unless he sees a proper prototype

**8/31/20 Weekly Group Meeting**

**Decisions:**

-	Going to keep on using InVision for design
-	As a group, we do not see a good reason for switching over to Figma
-	We are going to work on User Stories using Google Docs
-	Still haven’t decided how we are going to process the data; will brainstorm more as a group 

**Recaps + Plans:**

-	Thomas: reviewed Carolina Cloud Apps; finished project summary + project description; will focus on updating the website
-	Muyan: continue working on user stories and design
-	Teddy: reviewed Carolina Cloud Apps; continue working on user stories

**Actions items:**

-	Muyan: review Thomas’s project summary/description; review Thomas’s website changes; continue working on user stories and design; email Professor Hurlbert about Summer of Code work
-	Thomas: finalize project description; update the website with appropriate format changes
-	Teddy: review Thomas’s project summary/description; review Thomas’s website changes; continue working on user stories; draft meeting questions for Jacob

**Client Meeting (8/28)**

**Professor Hurlbert is envisioning 3 types of users:**

-	Scientists and ecologists: for many bird species, they know in general what the birds eat. However, when we start considering climate and land changes, we want to know how those changes will impact birds and their prey. Global changes will affect insects, and by exploring which birds rely on those specific insects, we can see the impact on birds. In addition, scientists don’t have the necessary technical skills to extract data from the flat excel file, so they need a better way to find out what birds eat. 
-	Non-scientists: people who are interested in birds and the natural world. Professor Hurlbert is going to publish this data set, and he is expecting press since this is the largest compilation of this type of data. This project can be a science outreach and reach others learn more about birds and ecology. Professor Hurlbert hasn’t figured out how people will discover this website (that is a different challenge). He wants this website to be easy and intuitive for non-scientists
-	Professor Hurlbert: he has already written summary scripts, but there some scripts/data visualization tools that he hasn’t written yet. He wants to be able to use this project in the future to demonstrate bird diet/ecology related topics.

**End notes:**

-	No authorization should be needed for the website (beginner friendly)
-	Mobile friendly to attract the non-scientist audience group since they will access the website on their mobile devices first. 
-	Professor Hurlbert prefers mySQL since decent amount of work has already been done on mySQL by his Summer of Code group.
-	Professor Hurlbert will try to forward us previous work from Summer of Code group

**8/28/20 Weekly Group Meeting**

**Went through Git Collaboration:**

-	Talked about git flow vs truck-based development (pros and cons of each)
-	We are going to use a trunk-based development workflow
-	There would be 1 master branch, and anytime someone wants to work on a new feature, they would check out a branch
-	When the feature branch is finished, they would rebase the master branch before merging in the feature branch
-	The workflow layout that we are following: https://www.endoflineblog.com/oneflow-a-git-branching-model-and-workflow
-	We aren’t going to focus much on release branches and hotfixes
-	Code review are required for every commit, and pull requests are required for every push
-	Look at a code review within 48 hours; let the team know if you can’t get to it

**Went through Code Style:**

-	Everyone agreed with the Code Style suggestions from last meeting
-	In addition to JavaScript Standard Style, we are also going to use ESLint (eslint.org)

**Next steps:**

-	Thomas has finished a description of the project, other team members should review it before adding it to the website
-	Upcoming meeting with Professor Hurlbert this afternoon; will focusing on clarifying project description + start thinking about user stories
-	Teddy will look more into Carolina Cloud App
-	Muyan shared his InVision design of the website so far; needs a lot of work; will look at other websites for ideas

**Action items:**

-	Teddy: review Thomas’s description, create Github project repository, look more into Carolina Cloud App
-	Muyan: review Thomas’s description, update team rules, continue working on InVision design
-	Thomas: finalize description and update the website, meet with Professor Hurlbert to clarify any misunderstandings

**Mentor Meeting (8/26)**

**Recap the meeting with Professor Hurlbert**: 

-	We were able to ask why he preferred certain requirements over others
-	Professor Hurlbert walked us through the PowerPoint and shared his vision with us
-	More details can be found under meeting notes w/ client (8/25)

**Should we learn R?**: 

-	It really depends; the timeline for this project is very tight, so we have to consider the pros and cons of the choices
-	It is okay not to learn R since it isn’t the only way

**Record of truth: should it be on the Excel spreadsheet or the website?**: 

-	Right now, Professor Hurlbert wants the website to be updated from the spreadsheet
-	However, this can become a problem when the user wants to upload his own studies
-	If the database and the spreadsheet have different information, which one do we trust?
-	Food for thought: when the user adds new studies to the website, have that upload/generate an excel spreadsheet

**The benefits of doing the design with InVision**: 

-	Making sure that all three of us are on the same page before we start coding
-	Making sure that we have an early deliverable for the client so he could offer any suggestions/disputes
-	This design will pretty much be the clickable prototype that is due on 9/13

**Data visualization**: 

-	This application is used for reporting
-	Review the PPT to see what Professor Hurlbert wants

**Prototype: web and mobile**: 

-	Difficulties with mobile apps and all of the different types of apps
-	Again, timeline for this project is tight, so we have to consider if making a prototype for the mobile device is worth it

**Saving the different iterations of the architecture diagrams**:
 
-	Useful in presentations to see the changes that have been made along the way
-	Demonstrates the different ideas that we came up with and the team’s growth

**Communication management**: 

-	Chucking up the work, so other people have the ability and authority to make decisions
-	Positive and negative feedbacks should both be welcomes
-	Roll forward with your mistakes; don’t backtrack; if one of the previous decisions turns out to be wrong, learn from it
-	Zoom open with no-one talking is useful since that be induce a collaboration environment
-	The benefits of using mural to share ideas with one another

**Git collaboration meeting**: 

-	We should document our git procedures to ensure that everyone is on the same page
-	Good reference point down the road

**Talk to Professor Hurlbert on the user stories**: 

-	When working on the project, always have the usage and target audience in mind; use that to make decisions
-	Use the user stories in future conversations with Professor Hurlbert
-	Maybe ask Professor Hurlbert 5 why’s on the mobile experience

**Introduction Meeting w/ Professor Hurlbert** (8/25)

Professor Hurlbert showed us the flat excel data + went over the column descriptions: 

-	Not all of the column fields have information; depends on what the study gave
-	Preys are identified with different levels, and the user should have the option to specify which level he wants when querying
-	Return outputs should be at the correct level; if that information is not available, return the highest available level (with appropriate logs)
-	‘Prey stage’ field also adds complexity to the query; however, prey part and prey stage could be concatenated when querying (look into this later)
-	‘Diet types’ specify how the diet distribution is measured; occurrence doesn’t sum (look at the maximum occurrence value)



**Questions on the requirement**:

**Why should the project be hosted on Carolina Cloud Apps?**:

-	Professor Hurlbert has other projects posted there
-	Free
-	Custom URL w/ UNC 
-	Associated w/ UNC
-	Size of the database really limits the hosting options
-	Professor Hurlbert is willing to explore other options, but he has to have the ability to tweak the code
-	Environment is hard to set up in Cloud Apps, but everything afterwards is easier

**Why mySQL?**:

-	This is what the Summer of Code group (previous group that worked on this project) did
-	Willing to explore other database options
-	Just making sure that the queries are returning the correct items (there are some messy queries)
-	Teddy suggests MongoDB 

**Cron job: Do we need database versions?**: 

-	Professor Hurlbert is still updating the flat excel sheet
-	He wants the website to update automatically
-	Excel flat file will be updated one study at a time (so multiple rows might be added)
-	The database is populated from the flat excel file

**Slides 3-6 on the PowerPoint**: 

-	Rough design
-	The homepage could just stop at “what does [animal] eat” and “what eats [animal]”
-	He envisioned different tabs for different queries, but the output could all appear on the same page

**Action items**: 

-	Professor Hurlbert: gather links from his Summer of Code team to see if there are useful information for us to use
-	Muyan: start looking at user stories, set up meeting going over git collaboration, work on design w/ InVision
-	Teddy: looking at InVision, database schema brainstorm, looking in Carolina Cloud Apps
-	Thomas: database schema brainstorm, looking in Carolina Cloud Apps
-	Recurring Client Meetings at 3pm on Fridays


**Recap**: 

-	Met with Jacob last week
-	Set up slack for internal communication
-	Decided that InVision could be a potential source for creating the design
-	Explore the proposal PDF and PPT to see if there is anything to ask Professor Hurlbert more about (5 why’s)

**Agenda**: 

-	Reviewed Trello board
-	Discussed personal strengths and weaknesses
-	Started working on team roles and team rules
-	Looked ahead to assignment 2

**Action items**: 

-	Teddy: setting up the website, journal, schedule, full stack drawing
-	Muyan: finish team rules including coding style and git collaboration (go over with Thomas and Teddy when complete), schedule a meeting w/ client
-	Thomas: invite client + mentor to Trello, tweet-sized project summary, longer project description

**Team roles**: 

-	Teddy: project manager, webmaster, tech lead, frontend lead, 
-	Muyan: client manager, design lead
-	Thomas: backend lead, infrastructure lead

**Team rules**:

-	Should a team member miss a meeting, he should notify other team members ASAP; best if other members are notified 24 hours in advance
-	Main source of communication among team members will be GroupMe
-	Try to check GroupMe at least twice a day (weekends included)
-	If there is a no response from a team member; other members will decide on the best action, and they might move on 

**Coding style**: 

- JavaScript Standard Style: https://standardjs.com/
- Log inputs when appropriate 
- When implementing new functions, add comment specifying purpose, parameter, and return types
- Camel naming structure

**Git collaboration**:

- Truck-based development: https://www.endoflineblog.com/oneflow-a-git-branching-model-and-workflow
- Check out new branches over using git stash
- Pull request and code reviews are situational, depending on the impact of the code changes
- Give team members 24 hours to review pull requests and code reviews

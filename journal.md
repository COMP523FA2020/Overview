---
title: "Journal"
permalink: /journal/
---
[Home](/Overview/) |  [Project](/Overview/project) | [Team](/Overview/team) | [Journal](/Overview/journal) | [Deliverables](/Overview/deliverables)

# Journals

**Mentor Meeting (8/26)**

***Recap the meeting with Professor Hurlbert: 

-	We were able to ask why he preferred certain requirements over others
-	Professor Hurlbert walked us through the PowerPoint and shared his vision with us
-	More details can be found under meeting notes w/ client (8/25)

***Should we learn R?: 

-	It really depends; the timeline for this project is very tight, so we have to consider the pros and cons of the choices
-	It is okay not to learn R since it isn’t the only way

***Record of truth: should it be on the Excel spreadsheet or the website?***: 

-	Right now, Professor Hurlbert wants the website to be updated from the spreadsheet
-	However, this can become a problem when the user wants to upload his own studies
-	If the database and the spreadsheet have different information, which one do we trust?
-	Food for thought: when the user adds new studies to the website, have that upload/generate an excel spreadsheet

***The benefits of doing the design with InVision: 

-	Making sure that all three of us are on the same page before we start coding
-	Making sure that we have an early deliverable for the client so he could offer any suggestions/disputes
-	This design will pretty much be the clickable prototype that is due on 9/13

***Data visualization: 

-	This application is used for reporting
-	Review the PPT to see what Professor Hurlbert wants

***Prototype: web and mobile: 

-	Difficulties with mobile apps and all of the different types of apps
-	Again, timeline for this project is tight, so we have to consider if making a prototype for the mobile device is worth it

***Saving the different iterations of the architecture diagrams:
 
-	Useful in presentations to see the changes that have been made along the way
-	Demonstrates the different ideas that we came up with and the team’s growth

***Communication management: 

-	Chucking up the work, so other people have the ability and authority to make decisions
-	Positive and negative feedbacks should both be welcomes
-	Roll forward with your mistakes; don’t backtrack; if one of the previous decisions turns out to be wrong, learn from it
-	Zoom open with no-one talking is useful since that be induce a collaboration environment
-	The benefits of using mural to share ideas with one another

***Git collaboration meeting: 

-	We should document our git procedures to ensure that everyone is on the same page
-	Good reference point down the road

***Talk to Professor Hurlbert on the user stories***: 

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

***Why should the project be hosted on Carolina Cloud Apps?***:

-	Professor Hurlbert has other projects posted there
-	Free
-	Custom URL w/ UNC 
-	Associated w/ UNC
-	Size of the database really limits the hosting options
-	Professor Hurlbert is willing to explore other options, but he has to have the ability to tweak the code
-	Environment is hard to set up in Cloud Apps, but everything afterwards is easier

***Why mySQL?***:

-	This is what the Summer of Code group (previous group that worked on this project) did
-	Willing to explore other database options
-	Just making sure that the queries are returning the correct items (there are some messy queries)
-	Teddy suggests MongoDB 

***Cron job: Do we need database versions?***: 

-	Professor Hurlbert is still updating the flat excel sheet
-	He wants the website to update automatically
-	Excel flat file will be updated one study at a time (so multiple rows might be added)
-	The database is populated from the flat excel file

***Slides 3-6 on the PowerPoint***: 

-	Rough design
-	The homepage could just stop at “what does [animal] eat” and “what eats [animal]”
-	He envisioned different tabs for different queries, but the output could all appear on the same page

***Action items***: 

-	Professor Hurlbert: gather links from his Summer of Code team to see if there are useful information for us to use
-	Muyan: start looking at user stories, set up meeting going over git collaboration, work on design w/ InVision
-	Teddy: looking at InVision, database schema brainstorm, looking in Carolina Cloud Apps
-	Thomas: database schema brainstorm, looking in Carolina Cloud Apps
-	Recurring Client Meetings at 3pm on Fridays


***Recap***: 

-	Met with Jacob last week
-	Set up slack for internal communication
-	Decided that InVision could be a potential source for creating the design
-	Explore the proposal PDF and PPT to see if there is anything to ask Professor Hurlbert more about (5 why’s)

***Agenda***: 

-	Reviewed Trello board
-	Discussed personal strengths and weaknesses
-	Started working on team roles and team rules
-	Looked ahead to assignment 2

***Action items***: 

-	Teddy: setting up the website, journal, schedule, full stack drawing
-	Muyan: finish team rules including coding style and git collaboration (go over with Thomas and Teddy when complete), schedule a meeting w/ client
-	Thomas: invite client + mentor to Trello, tweet-sized project summary, longer project description

***Team roles***: 

-	Teddy: project manager, webmaster, tech lead, frontend lead, 
-	Muyan: client manager, design lead
-	Thomas: backend lead, infrastructure lead

***Team rules***:

-	Should a team member miss a meeting, he should notify other team members ASAP; best if other members are notified 24 hours in advance
-	Main source of communication among team members will be GroupMe
-	Try to check GroupMe at least twice a day (weekends included)
-	If there is a no response from a team member; other members will decide on the best action, and they might move on 

***Coding style***: 

- JavaScript Standard Style: https://standardjs.com/
- Log inputs when appropriate 
- When implementing new functions, add comment specifying purpose, parameter, and return types
- Camel naming structure

***Git collaboration***:

- Truck-based development: https://www.endoflineblog.com/oneflow-a-git-branching-model-and-workflow
- Check out new branches over using git stash
- Pull request and code reviews are situational, depending on the impact of the code changes
- Give team members 24 hours to review pull requests and code reviews


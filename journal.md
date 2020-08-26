---
title: "Journal"
permalink: /journal/
---
[Home](/Overview/) |  [Project](/Overview/project) | [Team](/Overview/team) | [Journal](/Overview/journal) | [Deliverables](/Overview/deliverables)

# Journals

**Introduction Meeting w/ Professor Hurlbert** (8/25)

Professor Hurlbert showed us the flat excel data + went over the column descriptions: 

-	Not all of the column fields have information; depends on what the study gave
-	Preys are identified with different levels, and the user should have the option to specify which level he wants when querying
-	Return outputs should be at the correct level; if that information is not available, return the highest available level (with appropriate logs)
-	‘Prey stage’ field also adds complexity to the query; however, prey part and prey stage could be concatenated when querying (look into this later)
-	‘Diet types’ specify how the diet distribution is measured; occurrence doesn’t sum (look at the maximum occurrence value)

**Questions on the requirement**:

**Why should the project be hosted on Carolina Cloud Apps?**:

o	Professor Hurlbert has other projects posted there
o	Free
o	Custom URL w/ UNC 
o	Associated w/ UNC
o	Size of the database really limits the hosting options
o	Professor Hurlbert is willing to explore other options, but he has to have the ability to tweak the code
o	Environment is hard to set up in Cloud Apps, but everything afterwards is easier

**Why mySQL?**:

o	This is what the Summer of Code group (previous group that worked on this project) did
o	Willing to explore other database options
o	Just making sure that the queries are returning the correct items (there are some messy queries)
o	Teddy suggests MongoDB 

**Cron job: Do we need database versions?**: 

o	Professor Hurlbert is still updating the flat excel sheet
o	He wants the website to update automatically
o	Excel flat file will be updated one study at a time (so multiple rows might be added)
o	The database is populated from the flat excel file

**Slides 3-6 on the PowerPoint**: 

o	Rough design
o	The homepage could just stop at “what does [animal] eat” and “what eats [animal]”
o	He envisioned different tabs for different queries, but the output could all appear on the same page

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


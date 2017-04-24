# GraphTheory Year 3 Project 2017

## Project Overview
This Repo is for a Project for my 3rd year Module Graph theory. The aim of this project is to take information from our timetable system 
and represent this information on a informative and easy to read graph. This graph would then be used for presentation using it to explain how the timetable works
and why graphing it out and detailing it visually is a great way to go about solving this problem.
This project was done using <a href="https://neo4j.com/" style=""> Neo4J </a>
### What is <a href="https://neo4j.com/" style=""> Neo4J </a> ?
<a href="https://neo4j.com/" style=""> Neo4J </a> is a highly scalable native graph database that leverages data relationships as first-class entities, helping enterprises build intelligent applications to meet today’s evolving data challenges. It is perfect for taking vast amounts of information and representing them in sleak perfect graphs.
The graphing of this information is done using:
* Nodes 
* Relationships
* Labels
* Rel types
* Properties

## Queries
To create and use these components in Neo4J you use cypher queries.
#### Examples of Queries used
##### For a lecturer node
CREATE (n:Lecturer {Name: 'Ian Mcloughlin' }) RETURN n 
##### For a Module node
CREATE (n:Modules {Module: 'Graph Theory' }) RETURN n
##### For a Room node
CREATE (n:Rooms {room: 'PF15' }) RETURN n
##### For creating relationships
MATCH (a:Lecturer {Name: 'Ian Mcloughlin' }), (b:Modules {Module: 'Graph Theory'}) 
MERGE (a)-[:`Lectures`]->(b)

## Dev Diary 
Before this module I had never heard of Neo4J so like most of this course has been it was a learning experience. Making graphs and navigating the different parts of this whole thing was interesting. Though it being interesting like any assigment it was tasking and had its pressures. I'm not the best at sql orientated languages so navigating this and writing correct queries took many attempts. My approach was to just go at my graph first and create it from looking at the time table and breaking that information down into the different components of Neo4J and putting it all together to form a somewhat cooherant graph. The way I took this project was to take my current timetable for this semester and represent it on the graph. As seen below in the screenshots is the results of my attempt. If I was to do this again I'd maybe take a larger portion of the time table but less detailed, maybe take all the rooms and course but a bit broader strokes. Like every project I feel I could have done better or approach or researched better as there is always room to improve in everything. Though I'm happy with my attempt though the graph unorganised can look very messy. This project also helped me realise the benefits of using graphs to represent information and problem solve. I definitely feel that if I was to work in a group where there was a vast exchange of information working towards solving the problem, that I'd suggest to the team we use something like neo4j and look at the solving the problem through graph theory. This has for myself been one of the more thought provoking and interesting modules as I'm not the strongest at maths but has given me a different perspective on how to problem solve within IT and use different approaches. Taking what is given and using something that wouldn't exactly have come to mind before has helped me learn alot more and will strongly consider using something like this in the future when tackling other assignments and problems.

## Screenshots Of My Graph
### Entire Graph
![alt text](http://imgur.com/3DAh3nT.png "Main Graph")
### Rooms
![alt text](http://imgur.com/nrH1xT2.png "Rooms")
### Lecturers
![alt text](http://imgur.com/uSfa01n.png "Lecturers")
### Modules
![alt text](http://imgur.com/2SksXRN.png "Modules")
### Groups
![alt text](http://imgur.com/isQPJpO.png "Groups")
### Days
![alt text](http://imgur.com/XMwfKLu.png "Days")

## References
https://neo4j.com/use-cases/

http://stackoverflow.com/questions/19624414/delete-node-and-relationships-using-cypher-query-over-rest-api

http://stackoverflow.com/

http://timetable.gmit.ie/sws1617/(S(cflmi0555cqhk4ida3a2mvvh))/default.aspx


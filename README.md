For dashboard solution look at what gokay did with git 

Important:
Task 1: mention that the FAIR is complied to via GitHub repository 

Task 2: explain why everything is in 3rd NF. 
--> argue which data you ultimately include due to data minimisation 

Task 4: add the meta data part 
--> clean the data; note that the quotes in importing a cvs must be the right for characters used; also the separation is relevant!!

Task 5: compliance 
jsut some descripiteves and the project set up here for data management 
test test test change

Lecture 4 slides wrt that our db is fair compliant and thus also gdpr compliant 

For task 5 data compliance add and look at lecture 4; so the slides and gdpr


Gdpr, principle I) lawfulness, transparency, legal basis
The general legal basis of this is research. Additionally It is anonymised.
Important; mention that even though you deal with American data, you want to be fair compliant
As such: the anonymousiation from the get go (you only see case) so it is by design and default
. So because data is anonymised wrt to location, time , address and rqndomly  randomised it is by default 
Fair compliant.
Additionally, the data is public data and anonymised properly
Consent is not necessary here 

Gdpr, principle II) purpose limitation
Write in the Task5 that you you defined the purpose
In part 1 of the report and this way the data will be used 
The general purpose is to analyse crime 
--> important define the time limit during which you use the data
--> except for research!!!
--> put the data into cloud to make it save! 
--> encrypt the data file!! 
--> in sql lite db browser; when creating the database set a password; go to tools, set enrcptyion, cipher!!!
--> also mention that you encrypt the local file.

Gdpr, principle III) restrict and limit data (departmentize;
Use anonymouziqtion/randomization or pseudomizatuon; important document what you do!!!
Principle 3 is: integrity and confidentiality! 
But also not a problem in the assignment 


IMPORTANT: the data source was the university who already pre processed the data
To be gdpr compliant! So this is the data source and the data contact

But we aggregate and crime ids are mixed... so not connectable 

Gdpr, principleIV) limit data that you use
Principle: data minimisation! Make a choice which data you keep

Based on the outlined questions you need the following data
So only keep the defined data that you need for your question; based on 
The purpose defined in part 1 and upon request by Chicago pd 


Gdpr, principle V) data quality principle!!!
Important: mention versioning!!! Wrt versioning of the data.
--> STORAGE LIMITATION PRINCIPLE!!
 Task 4: outliers in coordinates 


Use triggers that restricts deletions, restrict access, log when someone uses it; set up dashboard  ; also prevent deletions via cascade 



Task 5: 
- outliers in the coordinates; beats mixing with wrong districts; date missing; location missing

- important: create an index for certain dates and seasons of relevance

- important: create a trigger for reading in data: the trigger  should look and log information for crime instances that do not have location (and look whether these instances are crimes without a location such a s financial crime)

- use indexes to speed up one of the answers in part 1; a good index might be to index evil crimes (eg homocides) and not index crimes that are not too bad. 

- triggers are used to data integrity; CREATE A MASTER FILE THAT REPORTS ALL CHANGES TO DATABASE!!
Regarding the master file: also create a log of IMPORTING DATA;
Additionally: create a trigger that logs a query to identify the user;
Example of logging when data is added to db - the VALUES define the action such as:(NEW.ProjectID, datetime(), 'INSERT NEW PROJECT'); NEW.ProjectID is used to create a new value

--> remember a delete and add logging is in the exercises 
Example of trigger logging was when data was changed (such as delete)
Todo: create a small DB next to the project database with a master table and subsequent tables that have a

Example of logging when query was done 


- important for task 5: restrict deletion of instances so that data integrity is warranted;

Create index for missing data being excluded


Task 6 look at examples from week 4; lecture 4 exercises for window functions ; don't forget to create views for variables and use indexes to speed up the queries 

Task 6--- provide a ranking of district and then by frustrier by best which has most crime etc using window function.


L4practice hour

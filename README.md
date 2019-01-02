<img align="right" src='http://www.aisp.sg/images/APP/ISS.jpg' width=25%>

## Machine Reasoning Workshops & References

**This [Machine Reasoning (MR)](https://www.iss.nus.edu.sg/executive-education/course/detail/machine-reasoning "Machine Reasoning") course is part of the Analytics and Intelligent Systems and Graduate Certificate in [Intelligent Reasoning Systems (IRS)](https://www.iss.nus.edu.sg/stackable-certificate-programmes/intelligent-systems "Intelligent Reasoning Systems") series offered by [NUS-ISS](https://www.iss.nus.edu.sg "Institute of Systems Science, National University of Singapore").**

**Lecturer: [GU Zhan (Sam)](https://www.iss.nus.edu.sg/about-us/staff/detail/201/GU%20Zhan "GU Zhan (Sam)")**

[![alt text](https://www.iss.nus.edu.sg/images/default-source/About-Us/7.6.1-teaching-staff/sam-website.tmb-.png "Let's check Sam' profile page")](https://www.iss.nus.edu.sg/about-us/staff/detail/201/GU%20Zhan)

**zhan.gu@nus.edu.sg**

---

### Open and refer to file: S-MR Workshop Guide.pdf

---

Institute of Systems Science

National University of Singapore

GRADUATE CERTIFICATE

INTELLIGENT REASONING SYSTEMS

Workshop Project (Continuous Assessment) Guide

Subject: Machine Reasoning


•	Source impactful real life business scenario for workshop project. 
•	Conduct comprehensive research and reference reading.
•	Make your own reasonable assumptions where necessary.


### Workshop 1 Guide


KIE: Installation & Familiarity

http://www.kiegroup.org/

http://bit.ly/iss-vm

Once you get KIE product suite installed, it’s time to see some running use cases. The easiest way is to try one of the examples shipped with the platform, it will show typical path users take to design, build and execute business logic.


### Workshop 1.1 [ Individual ]
KIE system: New user creation using admin user: wbadmin

Role controls user’s access to KIE product suite (Workbench roles);
Group controls user’s access to bespoke business system developed by KIE Workbench/product suit (Task roles);
New user creation procedure:
•	Step 1 Create all new users, and assign them relevant Roles (No new Group is ready).
•	Step 2 Create new Group, and link created new users.
Reference https://github.com/IRS-MR/S-MR-Workshop/blob/master/S-MR-Workshop1/KIE-Users.xlsx


### Workshop 1.2 [ Individual ]
KIE example system: Evaluation process

Evaluation process is a business process that is human centric (heavily uses human actors to perform work) that defines a complete flow of activities to perform employee evaluation. This examples shows:
•	importing example project
•	building and deploying project
•	verifying deployment to execution server
•	executing process instance and work with human tasks
•	exploring reporting capabilities
Reference https://www.youtube.com/watch?v=-fxL2iioPRI


### Workshop 1.3 [ Individual ]
KIE system development 1: Build your ‘getting-started’ project from scratch
Building new project from scratch can give you an option to have a clean start where you design your process or case to fit your needs. This example shows:
•	creating new project
•	creating new asset - business process
•	build and deploy to execution server
•	execute process instance
Reference https://www.youtube.com/watch?time_continue=3&v=pdgj0hrF5rc


KIE system development 2: Enhance above ‘getting-started’ project
Enhance above system by adding a Staff data object & an UpdateStaffRole machine reasoning business rule task to update staff role based on certain conditions:
•	When staff role filed is empty, OR
•	When staff name is e.g. ‘Sam’ AND staff number is e.g. ‘65674’
•	Then update staff role to e.g. ‘Lecturer’
Reference https://github.com/IRS-MR/S-MR-Workshop/tree/master/S-MR-Workshop1/project-io/getting-started.zip


### Workshop 1.4 [ Individual ]
Reasoning system analysis & exploration: Housing & Development Board Build-To-Order Recommender
Reference https://github.com/IRS-MR/bto-recommender-system


### Workshop 2 Guide


### Workshop 2.1 [ Individual ]
KIE example system: Mortgage loan application process
Mortgage process is a business process that is a blended human actors and automated machine reasoning process that defines a complete flow of activities to perform home loan application and approval. 
Reference https://github.com/IRS-MR/S-MR-Workshop
S-MR-Workshop2/project-io/example-Mortgage_Process.zip	

Machine Reasoning Enhanced Mortgage loan application process 
New Business Rule Task: MortgageMachineReasoning
Create a new new ' MortgageMachineReasoning' business rule task to replace 'Qualify' Human Task for automated mortgage loan in-limit checking. 
Reference https://github.com/IRS-MR/S-MR-Workshop
S-MR-Workshop2/project-io/Mortgage_Process_ISS_MR.zip	

Reference https://www.youtube.com/watch?v=s_8rct45b84

Reference https://github.com/IRS-MR/S-MR-Workshop/tree/master/S-MR-Workshop2


### Workshop 2.2 [ Individual ]
Knowledge Modeling
Identify a business opportunity to use reasoning system
Study online documented knowledge source as knowledge acquisition
Compose knowledge models in spreadsheets

Candidate Project: HDB BTO; Airport Gate Assignment System (AGAS); DoReMi; and alike
Reference 
Workshop 1.3 [Individual] https://github.com/IRS-MR/bto-recommender-system
ANNEX 1 WORKSHOP PROJECT CANDIDATE	


### Workshop 3 Guide


### Workshop 3.1 [ Individual ]
Data-Mining Enhanced Mortgage loan application process
Data mining / Rule induction / Orange3 decision tree

Extract business rule from data using inductive reasoning, e.g. bank loan example
Enhance KIE home loan system using the discovered knowledge, based upon: 
•	Workshop 2.1 [ Individual ] Machine Reasoning Enhanced Mortgage loan application process
Export enhanced KIE system and prepare for individual submission
Reference 
Guided Decision Tables https://www.youtube.com/watch?v=qBgxVoc2qfw
https://github.com/IRS-MR/S-MR-Workshop/tree/master/S-MR-Workshop3
ANNEX 2 PROJECT CODE EXPORT & IMPORT USING KIE WORKBENCH
ANNEX 3 WORKSHOP PROJECT SUBMISSION	


[ Example solution ] Data-Mining Enhanced Mortgage loan application process

https://github.com/IRS-MR/S-MR-Workshop/blob/master/S-MR-Workshop3/Mortgage_Process_ISS_MR.zip

•	New Business Rule Task	: Mortgage Machine Reasoning DT
•	New Guided Decision Table	: mortgagemachinereasoningDT


Build & Deploy


Use/Test Case 1

1st stage Approved: $200,000 Mortgage Amount: within limit mortgage amount 200,000 >= property sale price 250,000 – down payment 50,000
2nd stage Approved: InLimitMR checked: applicant has job


Use/Test Case 2

1st stage Approved: $200,000 Mortgage Amount: within limit mortgage amount 200,000 >= property sale price 250,000 – down payment 50,000
2nd stage Approved: InLimitMR checked: jobless applicant owning a house


Use/Test Case 3

1st stage Approved: $200,000 Mortgage Amount: within limit mortgage amount 200,000 >= property sale price 250,000 – down payment 50,000
2nd stage Disapproved: InLimitMR unchecked: jobless applicant not owning a house


### Workshop 3.2 [ EEP Individual / MTech Group ]

Identify a relevant business scenario/problem. Propose and create a knowledge-driven machine reasoning system.
The proposed grand workshop project must develop, integrate, and demonstrate at least two out of following three technique groups: 
1.	Business knowledge/rule based reasoning techniques
2.	Business knowledge/process based reasoning techniques 
3.	Knowledge Discovery OR Data Mining techniques 
The submitted runnable system should have a graphical user interface for end user to input or update data to execute different business use cases, e.g. Web or KIE form based user interface. And to display system output results in a user friendly manner. (Output console log is not considered user friendly.)

Grand project phase 1: Initialization 
Form team (MTech Thru-Train: 4 to 6 persons per project team)
Solicit business scenario / MVP
Design knowledge models
[Workshop 4] System Development / SDLC
[Workshop 4] MVP delivery & Documentation
Reference 
ANNEX 1 WORKSHOP PROJECT CANDIDATE
Workshop 2.2 [ Individual ] Knowledge Modeling	


### Workshop 4 Guide


### Workshop 4.1 [ EEP Individual / MTech Group ]
Grand project phase 2: Development  
[Workshop 3] Form team (MTech Thru-Train: 4 to 6 persons per project team)
[Workshop 3] Solicit business scenario / MVP
Design knowledge models
System Development / SDLC
MVP delivery & Documentation
Reference Workshop 3.2 Grand project phase 1: Initialization	

Grand project phase 3: MVP Delivery  
EEP & MTech Stackable: Submission due by 23:59 on last lecture date
MTech Thru-Train: Submission due by 23:59 on last lecture day + 14 
Reference 
ANNEX 2 PROJECT CODE EXPORT & IMPORT USING KIE WORKBENCH
ANNEX 3 WORKSHOP PROJECT SUBMISSION	

### ANNEX 1 WORKSHOP PROJECT CANDIDATE

### Workshop Project Candidate One

Airport Gate Assignment System (AGAS)

Faced with intense competition from major airports in the region, The Best Airport (TBA) needs to enhance the quality and efficiency of its airport services so that planes can have a faster turn-around. This improved throughput will definitely make its customers (the airlines) happy and to be firmly rooted to TBA. With some 5,000 flight arrivals each week, the assignment of aerobridges (or simply “gates”) is becoming increasingly complex and time consuming. Efficiency in gates assignment is crucial for TBA to remain as the airport of choice for all major airlines. You are a TBASU (TBA Strategic Unit) project specialist who is tasked to work on this important assignment.

The following is a transcript from your interview with Mr. Lim, the domain expert in gates scheduling:

You:	Mr. Lim, what is the first step in the assignment of a gate to an incoming flight?

Mr. Lim:	Well, flight information sends me a schedule of all incoming and outgoing flights for a particular day, at least 24 hours in advance for me to assign gates and service units to all flights. My first step is to prioritize all the flights, according to type - international or domestic, number of passengers and refueling needs. The number of passengers and refueling needs will determine how much time is needed, and thus how long the gate will be occupied. Another constraint is the amount of time before the plane has to depart. The top priority flight will be taken care of first. My job is to match a gate to an incoming flight for disembarkation of passengers and providing services for the aircraft.

You:	Is there a systematic procedure that you use for gate assignment?

Mr. Lim:	I 'm not sure what you mean by systematic, but what I do is, I determine the services required by an aircraft, and assign a service unit (SU) which is able to provide those services, to a gate. Obviously, both the SU and the gate must be free or available. I get this information from the Gates Operation System which is updated in real-time. But this assignment is not as simple as it sounds. Each gate has a max passenger handling capacity, so we need to know the number of passengers coming in. A gate is also reserved for either domestic or international flights. A gate is also limited by its capability of supporting the required services.

You:	Could you clarify this further with an example?

Mr. Lim:	OK, suppose that an aircraft needs catering and cleaning. Then we must look for a gate that is capable of supporting those 2 services. However, we also try to minimize wastage, in the sense that we do not want to assign a gate which is capable of supporting all 3 services, when only 2 are needed. We should try to save that gate for the time when all 3 services are needed.

You:	Let me recap: An SU can provide one or more services, like cleaning, catering and refueling depending on the needs of the aircraft. And the gate must be able to support the chosen SU.

Mr. Lim:	Correct. 

You:	So you are assigning SUs to a gate, and a gate to an aircraft? 

Mr. Lim:	You got it!

You:	Do all aircraft need the same services?

Mr. Lim:	No. But if a particular service is needed, then it is mandatory that a gate providing that service is assigned to the aircraft.

You:	Can you give me an example?

Mr. Lim:	Certainly. Suppose that cleaning, refueling and catering are needed. The ideal situation would be to assign SU-101, for example, which provides all 3 services. But suppose SU-101 is not available, then we need to look for free SU, say SU-104 which provides catering and cleaning, and SU-105 which provides refueling and cleaning. SU-104 would be assigned to provide the catering and cleaning, but refueling can come from SU-105. In this case there is a redundancy, which cannot be avoided. An SU can only be assigned to one flight and hence one gate only at any one time.

You:	How do you find out what services are required by an incoming flight?

Mr. Lim:	Cleaning is always needed. Refueling is determined by the remaining fuel level, and catering of meals depends on the duration of the next outgoing flight.

You:	And how do you compute how much fuel the aircraft needs for the flight out?

Mr. Lim:	We have a set of tables (pointing to the laminated papers) to refer to. We also use the tables to determine catering needs as well as to do the prioritization of flights that I mentioned earlier.

You:	I think I’ve taken too much of your time. Can I come back to you tomorrow to verify my understanding of what we discussed today? Thank you, Mr. Lim.



[End of Interview]


### Workshop Project Candidate Two

DoReMi Books Inc.
1. 	Background
DoReMi Books is a company that specializes in the supply and sale of classical music scores and music books in the USA with subsidiaries in the major cities of each of the 50 states. An important line of business for the company is the supply of music books to music schools. These schools buy books in bulk for their students and are given special bulk-package discounts. Sales to music schools constitute 30% of the annual revenue of DoReMi.
The organization structure of the company is shown below.
 
2. 	Business Process & Improvement 
As the company started in 1955 (and is now 57 years old), some of its business processes are manual and rather traditional. The company is now facing strong competition from its competitors (both new and old), who have embraced online and internet sales as the new way of interacting and transacting with their customers. 
In response to the new challenges brought on by online sales transactions, the Chief Executive Officer (CEO), Peter Lee, asked a consultant to conduct a business process improvement exercise to revamp their music books sale transaction and order handling process as well as introduce improved stock and inventory planning and management capabilities. One of the key outcomes of this exercise was a new order handling process and the introduction of an internet sales transaction system, including an advanced business intelligence module for optimal stock inventory and warehousing forecasting. 
After a period of process analysis and redesign, a new streamline process for online purchase from individual customers were defined. For bulk purchase, an automated workflow with automated inventory checks and approval was also established that can simplify the sales orders from music schools ordering in bulk. The process for handling orders from this client segment is simpler to implement as they have standard needs and also credit facilities already well established with DoReMi. The company is now ready to implement the new process and system. 
3. 	Planning Implementation and Rollout
In considering the plans for the implementation and rollout of the new process and system, the CEO asked all his department heads (Directors) to gather some informal feedback on this major business process change initiative. The following feedback was shared in the weekly management board meeting:
HR Director:	I am sensing some discomfort among the staff. The union has also mentioned about some talk of a rumour going around that the company is going on a down-sizing exercise and people will be made redundant once the new process and system is operationalised. This revamp thing that we are planning needs to be handled with care. I am hearing of head-hunters enquiring about our top-performing sales people.
Director Sales: 	I am not aware about the rumour. But in my informal checks with my team leaders, some are asking why are we doing this? We are in the music books industry, and as you know, this is a rather niche area, with our product being mainly in the classical genre and highly specialized stuff. Why should we be bothered with this online talk? Our customers are likely to be in the adult age-group and would not be keen in online transactions anyway.
Director Packaging and Warehousing:	A high proportion of our workers in my department are of the older generations and they are also some of our most loyal and experienced workers. As you know, we do need some classical music background knowledge in our business. The new IT-enable process and business intelligent system may pose a technology challenge to my people. There is worry that the high-tech stuff will actually slow them down.
Director IT: 	We have a lean team in our IT department and it is a constant struggle to keep up with the demands and expectations of the business units across the various geographically dispersed subsidiaries. Any introduction of new large IT systems will need to be carefully planned as it may cause a degradation of the IT support service. On a more positive note, the IT staff members are actually looking forward to learning and working with new tools and technologies. They are asking how they can find out more on process improvement and redesign concepts and methodologies.

4. 	DoReMi Books Order Handling Process
1.. 	The customer service representative receives a call from the customer.
2.. 	Determine if the customer has an existing account.
2.1.	If the customer has an existing account:
2.1.1.	Record the account number.
2.1.2.	Record the order information.
2.1.3.	If the order is not within the auto-approval limit, send the order to Account Department for review. Otherwise, approve the order.
2.2.	If the customer does not have an account:
2.2.1.	Record customer information.
2.2.2.	Assign account number.
2.2.3.	Record order information.
2.2.4.	If the order is not within the auto-approval limit, send the order to Account Department for review. Otherwise, approve the order.
3..	If the order is auto-approved, the followings activities are performed in sequential order.
3.1.	Send the order information to the packaging department in warehouse.
3.2.	Packaging department packages the goods.
3.3.	Packaging department arranges for delivery.
3.4.	Packaging department informs the customer service representative.
4.	If the order is sent for review:
4.1.	Account Department reviews the order manually.
4.2.	Determine if the order is an acceptable credit risk.
4.2.1.	If the order is an acceptable credit risk:
4.2.1.1.	Send the order information to the packaging department in warehouse.
4.2.1.2.	Packaging department packages the goods.
4.2.1.3.	Packaging department arranges for delivery.
4.2.1.4.	Packaging department informs the customer service representative.
4.2.2.	If the order is not an acceptable credit risk:
4.2.2.1.	Account Department cancels the order.
4.2.2.2.	Notify the customer about the cancellation through the customer service representative.


5.	Business Issues to Be Considered in System Design
A.	DoReMi have an existing logistics application system but the users are not sure of the details of the process it carries out. This is because the logistics system is a black box since there is no documentation and the original IT/user project managers have left the company.
B.	There are many common tasks across the different departments in DoReMi. For example, there are common tasks to collect customer particulars, to collect their orders, to check their credit worthiness etc. Currently, the different departments in DoReMi do not always carry out these tasks in the same manner. DoReMi management would like to standardise and streamline these tasks so that they are carried out in the most productive way.
C.	DoReMi have many HR internal forms that need to be automated. Some have simple processes, e.g. fill in by applicant, and review by his supervisor and approval by the supervisor’s manager. Others were more complicated, e.g. fill in by applicant, and then route to different approving persons depending on the dollar amount.
D.	DoReMi is thinking of implementing a Print-On-Demand business process for the school bulk ordering of music scores (e.g. for music band use). This new business process will not need to keep an inventory of music scores. Instead, the Print-on-Demand process will perform high-volume in-house printing of the music scores as and when orders come in. This will help reduce warehouse storage space and costs.
E.	Many of the DoReMi managers gave the requirement that they wanted a tool that could help them with delegation of tasks and tracking of the task status for the various small projects that they need to manage.
F.	For music books, DoReMi purchases books from many different publishers. The processing of the publisher’s invoices currently takes a lot of manual effort and DoReMi management is hoping to automate this process. 
G.	There are many sales promotions (such as Christmas Sale, New Year Sale etc.) and the price of the books can change often depending on many factors. The IT department currently takes too long to make the changes to the system to cater for the frequent price changes.
H.	During peak hours, the cashier is not able to cope with the large number of customers as each payment takes some time (eg: credit card slip printing and signing) and this adds up when there are many customers. 


### Workshop Project Candidate Three

Housing & Development Board Build-To-Order Recommender

Convert and implement HDB BTO system using KIE product suite, e.g. Drools, jBPM, Task, Form user interface, and other relevant programming modules.
 

### ANNEX 2 PROJECT CODE EXPORT & IMPORT USING KIE WORKBENCH

Example: export KIE project Mortgage_Process_ISS_MR from work space MySpace

Review project settings to obtain project URL link

Export project from KIE Workbench

1.	Select a folder for exporting, example here uses /home/iss-user/iss-vm-program/is-intelligent-reasoning-systems/jboss/project-io
2.	Start a Terminal there, key in command git clone ssh://wbadmin@localhost:8001/MySpace/Mortgage_Process_ISS_MR
3.	Key in password ‘wbadmin’ for user wbadmin


Import project into KIE Workbench

1.	In KIE workbench, select/create a project Space, example here uses ISS-MR
2.	Click menu function ‘Import Project’
3.	For Repository URL, key in file:///home/iss-user/iss-vm-program/is-intelligent-reasoning-systems/jboss/project-io/Mortgage_Process_ISS_MR

Reference
https://developer.jboss.org/thread/269991
https://developer.jboss.org/thread/237411
https://developer.jboss.org/thread/252588


### ANNEX 3 WORKSHOP PROJECT SUBMISSION

Submission due by 23:59 on last lecture date (+ 14)
One delayed day = 10 marks deduction

1.	[MTech & EEP] Create Github repository for project submission
2.	[MTech] Download Github repository as a ZIP file, then upload to NUS LumiNUS / IVLE

Reference https://github.com/IRS-PM/Workshop-Project-Submission-Template


### The End of Workshop Project Guide

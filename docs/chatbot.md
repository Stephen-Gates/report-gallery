---
Title: "Chatbot questions"
---

!!! note "Work in progress"

# Chatbot questions :fontawesome-solid-robot:{: .grey }

A Chatbot is another way to answer questions. [Chatbots require development](https://www.youtube.com/watch?v=buq0Q-0vdcw&feature=youtu.be) so a limited number of questions may be implemented. Common questions[^1] are usually implemented first.

Chatbot questions may be:

- about the collection of factsheets, e.g. "How many applications do we have?"
- about a specific factsheet *name*, e.g. "Who is responsible for the application *Dynamics*?".  
- small talk to test the Chatbot's capabilities, e.g. "Are you a robot?” or "What can you do?"

The Chatbot will respond with:

- [the answer](../chatbot-answers/#answer), e.g. "*Alex Bailey* is responsible for the application *Dynamics 365*"
- a [clarifying question](../chatbot-answers/#clarifying-question), e.g. "Do you mean *Dynamics 365 Marketing* or *Dynamics 365 Field Service*?" 
- [how to access the answer](../chatbot-answers/#how-to-access-the-answer) if it can't be displayed, e.g. "To see a list of all applications and who is responsible, view the [Inventory][inventory]."
- an [apology](../chatbot-answers/#apology) for not answering the question, and a call to action e.g. "I'm sorry, I can only answer these [questions](../chatbot/#user-groups)."
- [small talk](../chatbot-answers/#small-talk) and a call to action, e.g. "I'm a very clever robot. Ask me something."


## User Groups

1. What user groups do we have? [^1]^,^[^2]^,^[^4]
    - Returns a count of level 1 user groups.  
    - Returns Factsheet cards for level 1 user groups ordered alphabetically.
1. Decompose the user group *Marketing*? [^1]^,^[^4]
    - Returns a count of the next level of user groups.  
    - Returns Factsheet cards for the next level of user groups ordered alphabetically.
1. Show me the user group *Direct Marketing*. [^1]
    - Returns a Factsheet card for the user group, e.g. Name, description, location, tags   
1. Which applications support user group *Direct Marketing*? [^1]^,^[^2]
    - Returns a count of used applications. 
    - Returns Application Factsheet cards ordered alphabetically.
    
<!-- hide uncommon questions for now       
1. Who is impacted by project *Cloud Migration*?
    - Returns a count of impacted user groups. 
    - Returns User Group Factsheet cards ordered alphabetically.  
-->

## Business Capabilities

1. What business capabilities do we have? [^1]^,^[^2]^,^[^4]
    - Returns a count of level 1 business capabilities.  
    - Returns Factsheet cards for level 1 business capabilities in alphabetical order.
1. Decompose the business capability *Human Resource Management*? [^1]^,^[^4]
    - Returns a count of the next level of business capabilities.  
    - Returns Factsheet cards for the next level of business capabilities ordered alphabetically.
1. Show me the business capability *Recruiting*. [^1]
    - Returns a Factsheet card for the business capability, e.g. Name, description, tags      
1. Which applications support business capability *Staff Recruitment*? [^1]
    - Returns a count of supporting applications. 
    - Returns Factsheet cards ordered alphabetically.
    
<!-- hide uncommon questions for now           
1. What business capabilities are impacted by project *Cloud Migration*?
    - Returns a count of impacted business capabilities. 
    - Returns Business Capability Factsheet cards ordered alphabetically.     
1. What is the IT cost of business capability *Human Resource Management*?
-->

## Processes

1. What processes do we have? [^1]^,^[^2]^,^[^4]
    - Returns a count of level 1 processes.  
    - Returns Factsheet cards for level 1 processes in alphabetical order. 
1. Decompose the processes *Manage Human Resources*? [^1]^,^[^4]
    - Returns the next level of processes under *Manage Human Resources* in alphabetical order.
1. Show me the process *Onboard Staff*. [^1]
    - Returns a Factsheet card for the process, e.g. Name, description, tags      
1. Who is responsible for process *Onboard Staff*? [^1]
    - Returns Process Factsheet card     
1. Which applications support process *Onboard Staff*? [^1]
    - Returns a count of supporting applications. 
    - Returns Application Factsheet cards ordered alphabetically. 

<!-- hide uncommon questions for now           
1. What processes are impacted by project *Cloud Migration*?    
-->

## Applications

<!-- Questions about the collection of Application factsheets -->

1. How many applications do we have?
    - Returns a count of Active and Phase out applications
1. What applications are tagged #Re-assess? [^1]^,^[^2]^,^[^3]
    - Returns a count of applications tagged #Re-assess. 
    - Factsheet cards are returned ordered by date the tag was applied.
1. Which applications are end-of-life this year? [^2]
    - Returns a count of applications that have an end&#8209;of&#8209;life lifecycle status within the calendar year. 
    - Factsheet cards are returned ordered by the end&#8209;of&#8209;life lifecycle status date.
1. Which applications are end-of-life this financial year? 
    - Returns a count of applications that have an end&#8209;of&#8209;life lifecycle status within the financial year. Factsheet cards are returned ordered by the end&#8209;of&#8209;life lifecycle status date.  
1. Which applications will become end-of-life this year? 
    - Returns a count of applications that have an end&#8209;of&#8209;life lifecycle status between today and the end of the  calendar year. 
    - Factsheet cards are returned ordered by the end&#8209;of&#8209;life lifecycle status date.    
1. Which applications will become active this year? 
    - Returns a count of applications that have an active lifecycle status between today and the end of the calendar year. 
    - Factsheet cards are returned ordered by the active lifecycle status start date.      
1. What applications are impacted by project *Cloud Migration*?
    - Returns a count of impacted applications. 
    - Factsheet cards are returned ordered alphabetically.
<!--  Questions about a specific Application factsheet -->
1. Show me application *Dynamics 365*? [^1]
    - Returns a Factsheet card for the application, e.g. Name, description, lifecycle dates, successor, responsible subscription(s), tags
    - Asks a clarifying question if the application cannot be uniquely identified.
1. Who is responsible for application *Dynamics 365*? [^1]
    - Returns a Factsheet card for the application.
    - Asks a clarifying question if the application cannot be uniquely identified.
1. Does application *Dynamics 365* process sensitive data? 
    - Returns a count of data objects classified as sensitive that are processed (CRUD) by the application.
    - Returns a Factsheet card for the data objects classified as sensitive that are processed by the application. Factsheet cards are returned ordered by data classification and then alphabetically.
1. Who uses application *Zoom*? [^1]   
1. What will replace application *Zoom*? [^1]
    - Returns a Factsheet card for the application.
    - Returns a Factsheet card for the successor application.
    - Asks a clarifying question if the application cannot be uniquely identified.

## Data

1. Show me the data object *Customer*. [^1]
    - Returns a Factsheet card for the data object showing name, description, data classification and responsible subscriptions.
1. Which applications use data object *Customer* 
    - Returns a count of applications using the data object.
    - Returns a Factsheet cards applications using the data object ordered first by Create, Update, Deleted operations, then Read operations, and second alphabetically.
    
<!-- hide uncommon questions for now   
1. Who is the Data Steward[^5] for the data object *Customer*?
    - Returns a Factsheet card for the data object.
1. What is the data classification of data object *Customer*? 
    - Returns a Factsheet card for the data object.
--> 
    

        
<!-- hide uncommon questions for now       
1. ~~Where is data object *Customer* stored?~~ [^6] 
--> 

<!--
## Interfaces
-->

## Projects 

1. What projects/programs do we have? [^2]^,^[^4]
    - Returns a count of level 1 projects.
    - Factsheet cards are returned for active, level 1 projects in alphabetical order. 
1. Decompose the project/program *IT Modernisation*? [^1]^,^[^4]
    - Returns a count of the next level projects.  
    - Factsheet cards are returned for the next level of projects in alphabetical order.
1. Show me project *Cloud Migration*?
    - Returns a Factsheet card for the project, e.g. Name, description, lifecycle dates, successor, responsible subscription(s), tags.

<!-- hide uncommon questions for now 
1. What is lifecycle of project *Cloud Migration* ? 
    - Returns a Factsheet card for the project with lifecycle dates promoted in the visual hierarchy. 
-->

<!-- hide uncommon questions for now
## IT Components

1. Show me IT Component *SQL Server*?
    - Returns a Factsheet card for the IT Component, e.g. Name, description, lifecycle dates, successor, responsible subscription(s), tags, location
1. Where is IT Component *SQL Server* located? 
    - Returns a Factsheet card for the IT Component
-->

## Technical Stack

1. What technical categories do we have? [^2]^,^[^4]
    - Returns a count of level 1 technical categories. 
    - Returns level 1 technical categories in alphabetical order. 
1. Decompose the technical category *Databases*? [^4]
    - Returns the next level of technical categories in alphabetical order.
1. What IT Components are in the technical category *Relational Databases*? 
    - Returns a count of IT Components.
    - Returns IT Component Factsheet cards ordered by resource classification (Approved, Conditional, Investigating, Retiring, Unapproved) 
1. What is our standard IT Component for the technical category *Relational Databases*? 
    - Returns a Factsheet card for the IT Component where the resource classification is Approved.

<!-- hide uncommon questions for now   
## Providers

1. Show me provider *Microsoft*?
    - Returns a Factsheet card for the provider, e.g. Name, description, lifecycle dates, responsible subscription(s), tags.
1. Who is the provider of IT component *Azure hosting*?
    - Returns a Factsheet card for the provider.
-->

<!-- hide uncommon questions for now   
## Data quality

1. Show my to dos.
1. Show my overdue to dos.  
1. Show my broken quality seals
-->

## Small talk

People like to test the limits of a Chatbot. It's good to [respond to small talk](../chatbot-answers/#small-talk).

### Greetings

1. How are you? / How are you doing/going?
1. What’s up?
1. Good morning/evening/afternoon/night
1. Tell me something
1. Ok / Yes / I’ll do that now
1. Hello, Thank you, Goodbye
1. How can you help me? / what can you do?
1. Hi, my name is……
1. Happy birthday!
1. I have a question / can you help me?

### Fun phrases

1. Do you know a joke? / You’re funny!
1. Do you love me? / I love you
1. Will you marry me? / Are you single?
1. Do you like people?
1. Does Santa Claus exist?
1. Are you part of the Matrix?
1. You’re cute / beautiful / handsome
1. Do you have a hobby?
1. You’re smart / clever / intelligent
1. Tell me about your personality

### Phrases from users that are NOT HAPPY

1. !#$#% (swear words)
1. You’re annoying / you suck / you’re boring/bad /crazy
1. I want to speak to a human / live agent / customer service
1. Don’t you speak English?!
1. I want the answer NOW!

### Testing questions 

1. Are you human? / Are you a robot?
1. What is your name?
1. How old are you? / What’s your age?
1. What day is it today?
1. What do you do with my data? / Do you save what I say?
1. Who made you?
1. Which languages can you speak?
1. What is your mother’s name?
1. Where do you live?
1. What’s the weather like today?
1. Are you expensive?
1. Who’s your boss / master?
1. Do you get smarter?


<!-- link reference: link "tool tip" -->
<!-- does link have a .. and/or / in front? https://www.mkdocs.org/user-guide/writing-your-docs/#linking-to-pages-->
<!-- on local using .. I can't go up a level, but I can on /site -->

[factsheet-map]: ../factsheet-map/ "Factsheet Map reports"
[factsheet-map-user-group]: ../factsheet-map/#user-group "User Group map"
[factsheet-map-business-capability]: ../factsheet-map/#business-capability "Business Capability map"
[factsheet-map-process]: ../factsheet-map/#process "Process map"
[factsheet-map-data-object]: ../factsheet-map/#data-object "Data Object map"
[factsheet-map-technical-stack]: ../factsheet-map/#technical-stack "Technical Stack map"

[landscape]: ../landscape/ "Landscape reports"
[landscape-application]: ../landscape/application-landscape-reports/
[landscape-application-user-group]: ../landscape/application-landscape-reports/#user-group 
[landscape-application-business-capability]: ../landscape/application-landscape-reports/#business-capability
[landscape-application-process]: ../landscape/application-landscape-reports/#process
[landscape-it-component]: ../landscape/it-component-landscape-reports/
[landscape-it-component-technical-stack]: ../landscape/it-component-landscape-reports/#technical-stack
[landscape-it-component-provider]: ../landscape/it-component-landscape-reports/#provider
[landscape-project]: ../landscape/project-landscape-reports/
[landscape-project-user-group]: ../landscape/project-landscape-reports/#user-group 
[landscape-project-business-capability]: ../landscape/project-landscape-reports/#business-capability
[landscape-project-process]: ../landscape/project-landscape-reports/#process

[matrix]: ../matrix/ "Matrix reports"
[application-matrix]: ../matrix/application-matrix-reports
[application-matrix-business-capability-user-group]: ../matrix/application-matrix-reports/#business-capability-user-group
[application-matrix-process-user-group]: ../matrix/application-matrix-reports/#process-user-group
[application-matrix-process-business-capability]: ../matrix/application-matrix-reports/#process-business-capability
[application-matrix-time-business-capability]: ../matrix/application-matrix-reports/#time-business-capability
[application-matrix-time-user-group]: ../matrix/application-matrix-reports/#time-user-group

[it-component-matrix]: ../matrix/it-component-matrix-reports/
<!-- 3 settings -->

[project-matrix]: ../matrix/project-matrix-reports
<!-- 5 settings -->


[roadmap]: ../roadmap/ "Roadmap reports"
[roadmap-application]: ../roadmap/application-roadmap-reports
[roadmap-it-component]: ../roadmap/it-component-roadmap-reports
[roadmap-project]: ../roadmap/project-roadmap-reports


[location]: ../location/ "Location reports"
[location-application-usage]: ../location/application-usage-report
[location-it-component-location]: ../location/it-component-location-report

[interface]: ../interface/ "Interface reports"
[interface-circle]: ../interface/interface-circle-map-report "Interface Circle Map report"
[data-flow]: ../interface/data-flow-diagram "Data Flow diagram"

[cost]: ../cost/ "Cost reports"
[cost-business-capability]: ../cost/business-capability-cost-report
[cost-project]: ../cost/project-cost-report
[cost-provider]: ../cost/provider-cost-report

[lifecycle-age]: ../metrics/lifecycle-and-age-report "Lifecycle and Age reports"
[portfolio]: ../metrics/ "Portfolio reports"
[portfolio-application]: ../metrics/application-portfolio-report/
[portfolio-project]: ../metrics/project-portfolio-report/
[portfolio-provider]: ../metrics/provider-portfolio-report/

[inventory]: ../inventory/ "Inventory"

[^1]: Common questions suggested to implement first. 
[^2]: Perhaps this will return too many factsheets to be useful? Return results in a meaning order. 
[^3]: Useful to inform people performing application upgrades that these make not be required.
[^4]: This question may be needed to help ask other questions if people aren't familiar with the factsheet names.

<!--
[^5]: "Data Steward" is a configured [subscription role](https://docs.leanix.net/docs/manage-subscription-roles) on the Data Object factsheet 
[^6]: Too complex.
-->

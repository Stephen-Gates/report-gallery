---
Title: "Chatbot questions"
---

!!! note "Work in progress"

# Chatbot questions :fontawesome-solid-robot:{: .grey }

A Chatbot is another way to answer questions. [Chatbots require development](https://www.youtube.com/watch?v=buq0Q-0vdcw&feature=youtu.be) so a limited number of questions may be implemented. Common questions are usually implemented first.

Chatbot questions may be:

- about the collection of factsheets, e.g. "How many applications do we have?"
- about a specific factsheet *name*, e.g. "Who is responsible for the application *Dynamics*?".  
- small talk to test the Chatbot's capabilities, e.g. "Are you a robot?” or "What can you do?"

The Chatbot will respond with:

- [the answer](/chatbot-answers/#answer), e.g. "*Alex Bailey* is responsible for the application *Dynamics 365*"
- a [clarifying question](/chatbot-answers/#clarifying-question), e.g. "Do you mean *Dynamics 365 Marketing* or *Dynamics 365 Field Service*?" 
- [how to access the answer](/chatbot-answers/#how-to-access-the-answer) if it can't be displayed, e.g. "To see a list of all applications and who is responsible, view the [Inventory][inventory]."
- an [apology](/chatbot-answers/#apology) for not answering the question, and a call to action e.g. "I'm sorry, I can only answer these [questions](/chatbot/#user-groups)."
- [small talk](/chatbot-answers/#small-talk) and a call to action, e.g. "I'm a very clever robot. Ask me something."


## User Groups

1. Which applications do user group *Customers* use?

## Business Capabilities

1. Which applications support business capability *Customer Management*?
1. What is the IT cost of business capability *Human Resource Management*?

## Processes

1. Who is responsible for process *Onboard Staff*?
1. Which applications support process *Define Project Portfolio*?
    1. Which business critical applications support process *Identify Customer*?

## Applications

1. How many applications do we have?
1. Show me application *Dynamics 365*?
1. Which applications will become end-of-life this year?
1. Which applications will become active this year?
1. Who is responsible for an application *Dynamics 365*?
1. Who uses application *Zoom*? 
1. What will replace application *Zoom*? 
1. What applications have changed to #contain?[^1]
1. What applications are impacted by project *Cloud Migration*?
1. Does application *Dynamics 365* process sensitive data? 
1. What is the IT cost of operating application  *Dynamics 365*?

## Data

1. Who is the Data Steward[^2] for the data object *Customer*?
1. What is the data classification? 
1. [How are data objects grouped?][factsheet-map-data-object]
1. [What applications manage or access data?](https://store.leanix.net/en/report-details/753b11a9-4e86-4fad-a840-f76341bad983/c7d772df-2988-4024-920f-fb732d95cedc) :octicons-link-external-16:{: .grey } 
    1. What applications manage or access sensitive data?
1. Where is data stored? <!-- /location/it-component-location-report -->
    1. Is any sensitive data stored in other countries? i.e.  Is there a sovereignty risk?

<!--
## Interfaces

1. [What interfaces do we use?][inventory] 
1. [Which applications provide or consume interfaces?][interface-circle]
1. [How does data flow between applications?][data-flow]
    1. How is it the data transported? e.g. by file or API
    1. What is the frequency of data flows? e.g. real-time, hourly, or daily
    1. What is the data classification?
    1. Which application provides the interface?
    1. Which applications consume the interface?

-->

## Projects 

1. [What projects do we have?][inventory]
    1. How are projects grouped? e.g. Portfolios, Programs, and Projects
1. [When will a project start or end?][roadmap-project]
1. What applications will be changed by a project? - *(Free Draw diagram? Use smart explorer for a single project)*
1. [What user groups are impacted by projects because of the applications they change?][landscape-project-user-group]
1. [What business capabilities are impacted by projects because of the applications they change?][landscape-project-business-capability]
1. [What processes are impacted by projects because of the applications they change?][landscape-project-process]
1. What is a project's budget? - *(factsheet?)*
1. [Is the project budget on track?][cost-project]
1. [Which projects provide the highest value at the lowest risk?][portfolio-project]

## IT Components

1. [What IT Components do we have?][inventory], what are their properties, and who manages them? 
1. [Where are IT Components located?][location-it-component-location]
1. What technology implements an application? IT Component matrix with Application children or data flow or free draw
1. [How is the technology portfolio planned to evolve year by year?](/matrix/it-component-matrix-reports/#time-technical-stack) 
    1. [What is the technology roadmap?][roadmap-it-component]
    1. [What projects are implementing the technology roadmap?][roadmap-project]
1. What are our technical standards (preferred product to perform a function)? IT Component landscape with resource classification view - not answering functional bit. Need resource classification between application and business capability
  1. Which are standard technologies and can we reuse a solution?
1. What is the  our technical standards (preferred product to perform a function)? IT Component landscape with resource classification view - not answering functional bit. Need resource classification between application and business capability
1. [Is there opportunity to consolidate technologies?][landscape-it-component-technical-stack]
1. How is an application hosted and how is this planned to evolve?
1. [What is the planned lifecycle of an IT component][roadmap-it-component]


## Technical Stack

1. [What technology categories do we use to classify IT components?][inventory]
1. [How are technology categories grouped?][factsheet-map-technical-stack]
1. [What IT components are preferred to implement a technology category?][landscape-it-component-technical-stack]
1. What is our standard for 

## Providers

1. Show me provider *name*?
1. Who is the provider of IT Component *name*?
1. How much be we spend with Provider *name*? 

<!-- 

## other

From https://www.leanix.net/en/product/use-cases/integration-architecture-management

1. Is the data flow compromised by outdated Applications?
1. Are the Applications technically suited for the specific purpose?
1. How critical are the Applications in the data flow?
1. Which Applications are using employee data?
1. Is any customer data stored outside Europe?
1. Are there conflicts in manipulating data ("CRUD")?
1. How is the information flow across the Application Portfolio?
1. How are Applications interacting with each other and how often?
1. Are certain Applications a point of failure due to their high number of interfaces?

from https://www.leanix.net/en/product/use-cases/application-portfolio-management

1. Spot insufficient or unreasonable Functional Fit in an instant.
1. Communicate Applications that are going to be replaced with a Successor Application.
1. Identify the highest priorities to tackle first and focus your investments.
1. In which Applications to invest?
1. How well are Business Capabilities supported by Applications?
1. Who is using Applications where: Do we have support gaps? Do we have redundancies?
1. Who is providing the Application: Is this an effective setup?
1. How does the Application portfolio evolve over time?
1. Is the Application portfolio in line with our strategic business priorities?

from https://www.leanix.net/en/product/use-cases/technology-risk-management

1. Insights into whether an Application and the Business Capability it supports are at risk is therefore derived from the underlying IT Components.
1. How many IT Components are redundant?
1. Which Applications are at risk as the underlying IT components are out of the lifecycle?
1. Which IT Components go Out-of-Life?
1. Which Countries are most affected by Tech Risk?
1. Which actions are planned to mitigate the risk by the individual Application owners?

-->

## Small talk

People like to test the limits of a chatbot. It's good to respond to smalltalk.

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

[^1]: As changing lifecycle to "Phase out" seems extreme when going shopping, we could try using resource classification between IT Component and Technical Stack. People say "Application" but in LeaniX it's "IT Component".
[^2]: "Data Steward" is a configured [subscription role](https://docs.leanix.net/docs/manage-subscription-roles) on the Data Object factsheet 

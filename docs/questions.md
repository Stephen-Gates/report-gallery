---
Title: "Questions you can answer using LeanIX reports"
---

??? note "Work in progress"
    - This list needed to be rationalised and link to report pages.
        - Decide if duplication is allow with question reported or re-phrased in another section
    - Try use:
        - "Where" questions for location reports
        - "How much" questions for cost reports
        - "Who" for User Group reports
        - "How" for hierarchies
        - "When" for roadmaps or time matrix reports
        - "What" first, then "Which"; 
    - Focus on the factsheet part of the question first, with views as sub-questions  
    - My leaning is to put the factsheet that provides the answer as the first part of the question but sometime this doesn't sound natural.
    - If questions are phrased how people commonly ask, then it will be easier to turn this resource into a [chatbot](https://stephen-gates.github.io/chatbot/site/). :fontawesome-solid-robot:{: .grey }
    - The questions below are arranged by the factsheets involved in answering the question. 
      - Questions answered by using a built-in view are shown as sub-questions. 
      - Where I don't know how best to phrase a question, there may be an alternative phrasing as a sub-question, marked with *[alternative]*. 
    - Check question list against:
        - [How to Answer the Top Questions of Enterprise Architecture Stakeholders](https://www.leanix.net/en/download/how-to-answer-the-top-questions-of-enterprise-architecture-stakeholders)
        - [Smart Enterprise Architecture Governance in an Agile World](https://www.leanix.net/en/download/smart-ea-governance-in-an-agile-world)
        -[24 Key Enterprise Architecture Views for the Financial Services Industry](https://www.leanix.net/en/download/24-enterprise-architecture-views-financial-services)
        - [Reshape your IT with 24 Key Enterprise Architecture Views](https://www.leanix.net/en/download/reshape-your-it-with-24-key-enterprise-architecture-viewpoints) - doesn't have questions.

# Questions you can answer 

The questions below are arranged by the main factsheet type involved in answering the question. 

Questions based on a view using tags are marked with :fontawesome-solid-tag:{: .grey }. Tags are unique to your LeanIX implementation. 


## User Groups

1. [What user groups are part of, or interact with, our organisation?][inventory]
    1. Which user groups are "internal" or "external" to our organisation? :fontawesome-solid-tag:{: .grey }   
1. [How are user groups structured?][factsheet-map-user-group] 
1. [What applications support user groups?][landscape-application-user-group] 
    1. Which applications do "external" user groups use? :fontawesome-solid-tag:{: .grey }   <!-- this requires an internal/external tag on the user group factsheet -->
1. [Where are application users located?][location-application-usage]

    
## Business Capabilities

1. [What business capabilities support our organisation?][inventory]
  1. How are business capabilities classified? For example: a,b,c :fontawesome-solid-tag:{: .grey }  
1. [How are business capabilities structured?][factsheet-map-business-capability]
1. [Which applications support business capabilities?][landscape-application-business-capability] 
    1. Which business capabilities are impacted when an application fails? 
1. [What is the IT cost of supporting business capabilities?][cost-business-capability]

## Processes

1. [What processes does our organisation perform?][inventory]
    1. Who are the stakeholders?
1. [How are processes structured?][factsheet-map-process]
1. [Which applications support processes?][landscape-application-process]
    1. What processes are impacted when an application fails?
    1. Which applications are business critical in supporting a process?

## Applications

<!-- Application factsheet only questions -->
1. [What applications do we have?][inventory]
    1. Who are the stakeholders?
    1. Who is responsible for an application?
1. [How many applications do we have?][inventory]
1. [When are applications planned to change?][roadmap-application]
    1. When will successor applications replace existing applications?  
<!-- Application × User Group factsheet questions -->
1. [What applications are used by a user group to support a business capability?][application-matrix-business-capability-user-group]
1. [What applications are used by a user group to perform a process?][application-matrix-process-user-group]
    1. Who is impacted when an application fails? - *(smart explorer)*
    1. Which applications are business critical for a user group? 
1. [Where are applications used?](location/application-usage-report)
<!-- Application × Business Capability factsheet questions -->
1. [Which applications support business capabilities?](landscape/application-landscape-reports) 
    1. Can applications supporting the same business capability be rationalised?
1. For a group of related functions, what is the overall driver for change, intent and roadmap? 
1. For applications implementing a group of related functions, what is the target application, roadmap, and what is the status of the roadmap plan? 
1. What applications are critical to support which business capabilities?
<!-- Application × IT Components factsheet questions -->
1. [What applications are at risk due to obsolescent underlying IT components?](matrix/application-matrix-reports/) 
1. What is the health of applications and what action is required? (TIME: Tolerate, Invest, Migrate, Enhance) based on functional and technical fitness survey and other inputs. 
1. In which applications should we invest, which divest?
1. [Where are applications hosted?](location/application-sourcing-report/)
<!-- ### A x Project -->
1. [What applications are impacted by projects?]() - free draw, project roadmap with applications as children
1. [Which projects impact applications?]() *[alternative]*
<!-- ### A x D x I -->
1. Does an application process any sensitive data, how is this data classified, where is it located? 
<!-- ### A x ITC x Provider  -->
1. [What is the IT cost of operating applications?][cost-provider]
<!-- ### Matrix  -->
1. [What applications are used to support a business capability used to perform a process?](matrix/application-matrix-reports/#process-user-group)
<!-- ### unknown  -->
1. For a group of related functions, what applications implement these, what is there status and roadmap? 
1. How does the application portfolio change over time (planned and proposed)? 
1. What changes have occurred in the application portfolio since the last reporting period? 
    1. applications added, retired, change in status, renamed, change in roadmap dates, change in intent, etc.
    1. resource classification change
    1. lifecycle date changes (new Active, new Phase-out, End-of-life)
<!-- ### metrics -->
1. [How many applications are active or being phased out each month?](metrics/lifecycle-and-age-report.md)
1. [How many applications became active each year?](metrics/lifecycle-and-age-report)
    

## Data

1. [What data objects do we use?][inventory]
    1. Who are the stakeholders?
    1. What is the data classification (i.e. confidentiality)? 
    1. What is the category of the data ("Master data", "Reference data", "Transactional data", "Metadata")? :fontawesome-solid-tag:{: .grey }  
1. [How are data objects structured?][factsheet-map-data-object]
1. [What applications manage or access data?](https://store.leanix.net/en/report-details/753b11a9-4e86-4fad-a840-f76341bad983/c7d772df-2988-4024-920f-fb732d95cedc) 
    1. What applications manage or access sensitive data?
1. Where is data stored? <!-- /location/it-component-location-report -->
    1. Is any sensitive data stored in other countries? i.e.  Is there a sovereignty risk?
1. [How does data flow between applications?][dataflow]

## Interfaces

1. [What interfaces do we use?][inventory] 
1. [Which applications provide or consume interfaces?][circle-map]

<!--
1. [How does data flow between applications?][data-flow]
    1. How is it the data transported? e.g. by file or API
    1. What is the frequency of data flows? e.g. real-time, hourly, or daily
    1. What is the data classification?
    1. Which application provides the interface?
    1. Which applications consume the interface?
-->

## Projects 

1. [What projects do we have?][inventory]
<!--    1. How are projects structured? e.g. Portfolios, Programs, and Projects. Not available in Factsheet Maps -->
1. [When will a project start or end?][roadmap-project]
<!-- 1. What applications will be changed by a project? *(Free Draw diagram? Use smart explorer for a single project)* -->
1. [What user groups are impacted by projects because of the applications they change?][landscape-project-user-group]
1. [What business capabilities are impacted by projects because of the applications they change?][landscape-project-business-capability]
1. [What processes are impacted by projects because of the applications they change?][landscape-project-process]
<!-- 1. What is a project's budget? - *(factsheet?)*  -->
1. [Is the project budget on track?][cost-project]
1. [Which projects provide the highest value at the lowest risk?][portfolio-project]

## IT Components

1. [What IT Components do we have?][inventory], what are their properties, and who manages them? 
1. [Where are IT Components located?][location-it-component-location]
1. What technology implements an application? <!--IT Component matrix with Application children or data flow or free draw -->
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
1. [How are technology categories structured?][factsheet-map-technical-stack]
1. [What IT components are preferred to implement a technology category?][landscape-it-component-technical-stack]


## Providers

1. [What providers do we use?][inventory]
1. [What IT components does a provider supply?][landscape-it-component-provider]
1. What is the risk of a provider?
1. [Is there an opportunity to reduce the number of providers we deal with by changing technologies](/matrix/it-component-matrix-reports/#technical-stack-provider)
1. [What is the total IT spend by provider?][cost-provider]
1. [Which provider relationships need closer management?][portfolio-provider]

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

[circle-map]: ../interface/ "Interface Circle map"
[dataflow]: ../dataflow/ "Data Flow diagram"

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

<!-- Glossary terms --> 

*[Reference data]: Reference data is data that is referenced and shared by a number of systems. Most of the reference data refers to concepts that either impact business processes - e.g. order status (CREATED | APPROVED | REJECTED ) - or is used as an additional standardised semantic that further clarifies the interpretation of a data record - e.g. employee job position (JUNIOR | SENIOR | VP | etc.)

*[Metadata]: Metadata is data that describes other data; it is the underlying definition or description of data. 

*[Master data]: Master Data is key business information that supports the transactions.
Master Data describes the customers, products, parts, employees, etc. involved in the transactions. It is commonly referred to
as Places (locations, geography, sites, etc.), Parties (persons, customers, suppliers, employees, etc.) and Things (products, items, material, vehicles, etc.).

*[Transactional data]: Transactional data describes business events.

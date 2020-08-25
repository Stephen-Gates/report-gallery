---
Title: "Questions you can answer with LeanIX reports"
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
    - Check question list against:
        - [How to Answer the Top Questions of Enterprise Architecture Stakeholders](https://www.leanix.net/en/download/how-to-answer-the-top-questions-of-enterprise-architecture-stakeholders)
        - [Smart Enterprise Architecture Governance in an Agile World](https://www.leanix.net/en/download/smart-ea-governance-in-an-agile-world)
        -[24 Key Enterprise Architecture Views for the Financial Services Industry](https://www.leanix.net/en/download/24-enterprise-architecture-views-financial-services)
        - [Reshape your IT with 24 Key Enterprise Architecture Views](https://www.leanix.net/en/download/reshape-your-it-with-24-key-enterprise-architecture-viewpoints) - doesn't have questions

# Questions you can answer with LeanIX reports

## User Groups

1. [What user groups are part of, or interact with, our organisation?][inventory]
1. [How are user groups organised in a hierarchy?][user-group-map] 
1. [Who uses which applications?][user-group-application-landscape]
1. [Where are users of applications located?](/location/application-usage-report)

## Business Capabilities

1. [What business capabilities support our organisation?][inventory]
1. [How are business capabilities grouped?][business-capability-map]
1. [Which business capabilities are supported by applications?][business-capability-application-landscape]  
    1. Which business capabilities are impacted when an application fails? 
1. [What is the IT cost of supporting business capabilities?](/cost/business-capability-cost-report)

## Processes

1. [What processes do we perform?][inventory]
    1. Who are the stakeholders?
1. [How are processes grouped?][process-map]
1. [Which processes are supported by applications?][process-application-landscape]
    1. What processes are impacted when an application fails?
    1. Which applications are business critical in performing a process?

## Applications

<!-- Application factsheet only questions -->
1. [What applications do we have?][inventory]
    1. Who are the stakeholders?
1. [When are applications planned to change?](/roadmap/application-roadmap-reports)
    1. When will successor applications replace existing applications?  
<!-- Application × User Group factsheet questions -->
1. [What applications are used by a user group to support a business capability?](/matrix/application-matrix-reports/#business-capability-user-group)
1. [What applications are used by a user group to perform a process?](/matrix/application-matrix-reports/#process-user-group)
1. Who is impacted when an application fails? - *(smart explorer)*
1. Which applications are business critical for a user group? 
1. [Where are applications used?](/location/application-usage-report)
<!-- Application × Business Capability factsheet questions -->
1. [Which applications support business capabilities?](/landscape/application-landscape-reports) - repeat BC3
    1. Can applications supporting the same business capability be rationalised?
1. For a group of related functions, what is the overall driver for change, intent and roadmap? 
1. For applications implementing a group of related functions, what is the target application, roadmap, and what is the status of the roadmap plan? 
1. What applications are critical to support which business capabilities?
<!-- Application × IT Components factsheet questions -->
1. [What applications are at risk due to obsolescent underlying IT components?](/matrix/application-matrix-reports/) 
1. What is the health of applications and what action is required? (TIME: Tolerate, Invest, Migrate, Enhance) based on functional and technical fitness survey and other inputs. 
1. In which applications should we invest, which divest?
1. Where are applications hosted?
<!-- ### A x Project -->
1. [What applications are changed or impacted by projects?]() - free draw, project roadmap with applications as children
1. [Which projects will change or impact applications?]() - free draw, project roadmap with applications as children
<!-- ### A x D x I -->
1. Does an application process any sensitive data, how is this data classified, where is it located? 
<!-- ### A x ITC x Provider  -->
1. [What is the IT cost of operating applications?](/cost/provider-cost-report)
<!-- ### Matrix  -->
1. [What applications are used to support a business capability used to perform a process?](/matrix/application-matrix-reports/#process-user-group)
<!-- ### unknown  -->
1. For a group of related functions, what applications implement these, what is there status and roadmap? 
1. How does the application portfolio change over time (planned and proposed)? 
1. What changes have occurred in the application portfolio since the last reporting period? 
    1. applications added, retired, change in status, renamed, change in roadmap dates, change in intent, etc.
    1. resource classification change
    1. lifecycle date changes (new Active, new Phase-out, End-of-life)
<!-- ### metrics -->
1. [How many applications are active or being phased out each month?](/metrics/lifecycle-and-age-report.md)
1. [How many applications became active each year?](/metrics/lifecycle-and-age-report)
    

## Data

1. [What data objects do we use?][inventory]
    1. Who are the stakeholders?
    1. What is the data classification? 
1. [How are data objects grouped?][data-object-map]
1. [What applications manage or access data?](https://store.leanix.net/en/report-details/753b11a9-4e86-4fad-a840-f76341bad983/c7d772df-2988-4024-920f-fb732d95cedc) :octicons-link-external-16:{: .external-link } 
    1. What applications manage or access sensitive data?
1. [Where is data stored?](location/it-component-location-report)
    1. Is any sensitive data stored in other countries? i.e.  Is there a sovereignty risk?

## Interfaces

1. [What interfaces do we use?][inventory] 
1. [Which applications provide or consume interfaces?][interface]  
1. [How does data flow between applications?][data-flow]
    1. How is it the data transported? e.g. by file or API
    1. What is the frequency of data flows? e.g. real-time, hourly, or daily
    1. What is the data classification?
    1. Which application provides the interface?
    1. Which applications consume the interface?

## Projects 

1. [What projects do we have?][inventory]
    1. How are projects grouped? e.g. Portfolios, Programs, and Projects
1. [When will a project start or end?](/roadmap/project-roadmap-reports)
1. What applications will be changed by a project? - *(Free Draw diagram? Use smart explorer for a single project)*
1. [What user groups are impacted by projects because of the applications they change?](/landscape/project-landscape-reports/#user-group)
1. [What business capabilities are impacted by projects because of the applications they change?](/landscape/project-landscape-reports/#business-capability)
1. [What processes are impacted by projects because of the applications they change?](/landscape/project-landscape-reports/#process)
1. What is a project's budget? - *(factsheet?)*
1. [Is the project budget on track?](/cost/project-cost-report/)
1. [Which projects provide the highest value at the lowest risk?](/metrics/project-portfolio-report)

## IT Components

1. [What IT Components do we have?][inventory], what are their properties, and who manages them? 
1. [Where are IT Components located?](location/it-component-location-report)
1. What technology implements an application? IT Component matrix with Application children or data flow or free draw
1. [How is the technology portfolio planned to evolve year by year?](/matrix/it-component-matrix-reports/#time-technical-stack) 
    1. [What is the technology roadmap?](/roadmap/project-roadmap-reports)
    1. What projects are implementing the technology roadmap?
1. What are our technical standards (preferred product to perform a function)? IT Component landscape with resource classification view - not answering functional bit. Need resource classification between application and business capability
  1. Which are standard technologies and can we reuse a solution?
1. What is the  our technical standards (preferred product to perform a function)? IT Component landscape with resource classification view - not answering functional bit. Need resource classification between application and business capability
1. [Is there opportunity to consolidate technologies?](/landscape/it-component-landscape/) 
1. How is an application hosted and how is this planned to evolve?


## Technical Stack

1. [What technology categories do we use to classify IT components?][inventory]
1. [How are technology categories grouped?][technical-stack-map]
1. [What IT components are preferred to implement a technology category?](/landscape/it-component-landscape/) 


## Providers

1. [What providers do we use?][inventory]
1. [What IT components does a provider supply?](http://localhost:8000/landscape/it-component-landscape-reports/#provider)
1. What is the aggregate risk around a provider?
1. [Is there an opportunity to reduce the number of providers we deal with by changing technologies](/matrix/it-component-matrix-reports/#technical-stack-provider)
1. [What is the aggregate IT spend by provider?](/cost/provider-cost-report/) 
1. [Which provider relationships need closer management?](/metrics/provider-portfolio-report)

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

## BTM

1. Is the application portfolio evolution aligned to strategic business priorities? Can't do


-->

<!-- link reference: link "tool tip" -->
<!-- does link have a .. and/or / in front? https://www.mkdocs.org/user-guide/writing-your-docs/#linking-to-pages-->
[factsheet-map]: /factsheet-map/index.md "Factsheet Map reports"
[user-group-map]: /factsheet-map/#user-group "User Group map"
[business-capability-map]: /factsheet-map/#business-capability "Business Capability map"
[process-map]: /factsheet-map/#process "Process map"
[data-object-map]: /factsheet-map/#data-object "Data Object map"
[technical-stack-map]: /factsheet-map/#technical-stack "Technical Stack map"

[landscape]: landscape/index.md "Landscape reports"
[user-group-application-landscape]: /landscape/application-landscape-reports/#user-group 
[business-capability-application-landscape]: /landscape/application-landscape-reports/#business-capability
[process-application-landscape]: /landscape/application-landscape-reports/#process

[matrix]: matrix/index.md "Matrix reports"
[roadmap]: roadmap/index.md "Roadmap reports"
[location]: location/index.md "Location reports"
[interface]: interface/interface-circle-map-report.md "Interface Circle Map report"
[data-flow]: interface/data-flow-diagram.md "Data Flow diagram"
[cost]: cost/index.md "Cost reports"
[lifecycle-age]: metrics/lifecycle-and-age-report.md "Lifecycle and Age reports"
[portfolio]: metrics/index.md "Portfolio reports"
[inventory]: inventory/index.md "Inventory"

---
Title: "Questions you can answer with LeanIX reports"
---

??? note "Work in progress"
    - This list needed to be rationalised and link to report pages.
    - Take inspiration from the How to Answer the [Top Questions of Enterprise Architecture Stakeholders](https://www.leanix.net/en/download/how-to-answer-the-top-questions-of-enterprise-architecture-stakeholders) poster."
    - do we allow variants questions? Marking them with a number at the end of the question^#^

# Questions you can answer with LeanIX reports

## User Groups

1. [What user groups do we have?](/inventory-reports)
1. [How are user groups organised in a hierarchy?](/factsheet-map-reports/#user-group) 
1. [Who uses what applications?](/landscape-reports/application-landscape-reports)^1^
    1. Who is impacted when an application fails? 
1. ~~[Who uses what applications to provide a business capability?](/matrix-reports/application-matrix-reports/#business-capability-user-group)~~ belongs in Application section
1. ~~[Who uses what applications within a process?](/matrix-reports/application-matrix-reports/#process-user-group)~~  belongs in Application section
1. ~~[How will user group's use of applications change over time?](/matrix-reports/application-matrix-reports/#time-user-group)~~  belongs in Application section
1. [Where are user groups using applications located?](/location-reports/application-usage-report)

## Business Capabilities

1. [What business capabilities do we have?](/inventory) 
1. [What business capabilities support our business?](/factsheet-map-reports/#business-capability)
1. [Which business capabilities are supported by applications?](/landscape-reports/application-landscape-reports)^2^ 
1. ~~[Who uses what applications to provide a business capability?](/matrix-reports/application-matrix-reports/#business-capability-user-group)* reword to have bc first? do we allow duplicate?~~ 
1. ~~[Which business capabilities, supported by an application, are used in a process?](/matrix-reports/application-matrix-reports/#business-capability-user-group)~~
1. ~~[How will the support of business capabilities by applications change over time?](/matrix-reports/application-matrix-reports/#time-business-capability)~~
1. Which applications need to improve to met the desired business capability maturity level? Is this a Functional Fitness question? 
1. [What is the IT cost of supporting a business capability?](/cost-reports/business-capability-cost-report)

## Processes

1. [What Processes do we have?](/inventory)
1. [How are our processes organised in hierarchies?](/factsheet-map-reports/#user-group)
1. [What processes are supported by which applications?](/landscape-reports/application-landscape-reports)^3^
    1. What processes are impacted when an application fails?
1. [Which applications support a business process?](/landscape-reports/application-landscape-reports)
1. [Who are the stakeholders involved in each process?](/inventory-reports)

## Applications

1. [What applications do we have?](/inventory)
1. [What applications support which user groups?](/landscape-reports/application-landscape-reports)^1^
1. [What applications support which business capabilities?](/landscape-reports/application-landscape-reports)^2^ 
    1. Can applications supporting the same business capability be rationalised?
1. [What applications support which processes?](/landscape-reports/application-landscape-reports)^3^
1. [What applications are at risk due to obsolescent underlying IT components?](/matrix-reports/application-matrix-reports/) 
1. [What applications are changed or impacted by which projects?]() - free draw, project roadmap with applications as children
1. [What applications are used by a user group to support a business capability?](/matrix-reports/application-matrix-reports/#business-capability-user-group)
1. [What applications are used by a user group to perform a process?](/matrix-reports/application-matrix-reports/#process-user-group)
1. [What applications are used to support a business capability used to perform a process?](/matrix-reports/application-matrix-reports/#process-user-group)
1. For a group of related functions, what applications implement these, what is there status and roadmap? 
1. [What is the application roadmap?](/roadmap-reports/application-roadmap-reports)
1. For a group of related functions, what is the overall driver for change, intent and roadmap? 
1. For applications implementing a group of related functions, what is the target application, roadmap, and what is the status of the roadmap plan? 
1. What is the health of applications and what action is required? (TIME: Tolerate, Invest, Migrate, Enhance) based on functional and technical fitness survey and other inputs. 
1. In which applications should we invest, which divest?
1. How does the application portfolio change over time (planned and proposed)? 
1. Is the application portfolio evolution aligned to strategic business priorities?
1. Does an application process any sensitive data, how is this data classified, where is it located? 
1. What is our cost structure?
1. [What is the IT cost of operating an application?](/cost-reports/provider-cost-report)
1. What applications are being phased out?
1. What applications are critical to support which business capabilities?
1. What changes have occurred in the application portfolio since the last reporting period? 
    1. applications added, retired, change in status, renamed, change in roadmap dates, change in intent, etc.
    1. resource classification change
    1. lifecycle date changes (new Active, new Phase-out, End-of-life)



## Data

1. [What Data objects do we have?](/inventory), what is their data classification and who manages them? 
1. [What is the data objects do we manage](/factsheet-map-reports/#data-object) and what is their data classification?
1. [Where is sensitive data stored? Is there a sovereignty risk?](location-reports/it-component-location-report) - *Filter by Data Classification.*
1. [What applications perform operations (CRUD) on data objects?](https://store.leanix.net/en/report-details/753b11a9-4e86-4fad-a840-f76341bad983/c7d772df-2988-4024-920f-fb732d95cedc) - *Custom report* 
1. [What applications manage sensitive data?](https://store.leanix.net/en/report-details/753b11a9-4e86-4fad-a840-f76341bad983/c7d772df-2988-4024-920f-fb732d95cedc) - *Custom report* or use [application matrix report](/matrix-reports/application-matrix-reports) with data classification view
1. [What Applications providers and consume data via interfaces?](interface-reports/interface-circle-map-report)
1. [How is sensitive data transferred through the IT landscape?](interface-reports/data-flow-diagram)

## Interfaces

1. [What Interfaces do we have?](/inventory) 
1. [What data flows between applications?](interface-reports/interface-circle-map-report/) 
1. [How does data flow through the IT landscape?](/interface-reports/data-flow-diagram/)
    1. How is it the data transported (File, API)?
    1. What is the frequency of the data flow (real-time, hourly)?
    1. Is the data sensitive?
    1. What applications provide or consume the data?


## Projects 

1. [What Projects do we have?](/inventory)
1. What applications are impacted by which projects? 
1. What initiatives plan to change the application portfolio?
1. Are any technology elements missing that are needed to support the proposed project portfolio? - unanswerable - human needed
1. What budget is planned for certain projects? - factsheet?
1. [Is the project budget on track?](/cost-reports/project-cost-report/)
1. [When will a project be completed?](/roadmap-reports/project-roadmap-reports)
1. [Which projects provide the highest value at the lowest risk?](/metrix-reports/project-portfolio-reports)

## IT Components

1. [What IT Components do we have](/inventory), what are their properties, and who manages them? 
1. [Where are IT Components located?](location-reports/it-component-location-report)
1. What technology implements an application? IT Component matrix with Application children or data flow or free draw
1. [How is the technology portfolio planned to evolve year by year?](/matrix-reports/it-component-matrix-reports/#time-technical-stack) 
    1. [What is the technology roadmap?](/roadmap-reports/project-roadmap-reports)
    1. What projects are implementing the technology roadmap?
1. What are our technical standards (preferred product to perform a function)? IT Component landscape with resource classification view - not answering functional bit. Need resource classification between application and business capability
  1. Which are standard technologies and can we reuse a solution?
1. [Is there opportunity to consolidate technologies?](/landscape-reports/it-component-landscape-reports/) 
1. How is an application hosted and how is this planned to evolve?


## Technical Stack

1. [What technology categories do we use?](/inventory)
1. [How are technology categories organised in a hierarchy to help classify IT components?](/factsheet-map-reports/#technical-stack)
1. [What are our preferred IT components to use in a technology category?](/landscape-reports/it-component-landscape-reports/) 


## Providers

1. [What Providers do we use?](/inventory)
1. Who is the provider of an application / technology? 
1. What is the aggregate risk around a provider?
1. Is there an opportunity to reduce the number of providers we deal with by changing technologies](/matrix-reports/it-component-matrix-reports/#technical-stack-provider)
1. [What is the aggregate IT spend by provider?](../cost-reports/provider-cost-report/) 

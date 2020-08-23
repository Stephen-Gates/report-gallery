---
Title: "Questions you can answer with LeanIX reports"
---

??? note "Work in progress"
    - This list needed to be rationalised and link to report pages.
    - Take inspiration from the How to Answer the [Top Questions of Enterprise Architecture Stakeholders](https://www.leanix.net/en/download/how-to-answer-the-top-questions-of-enterprise-architecture-stakeholders) poster."
    - do we allow variants questions? Marking them with a number at the end of the question^#^

# Questions you can answer with LeanIX reports

## User Groups

1. [What user groups are part of, or interact with, our organisation?](/inventory)
1. [How are user groups organised?](/factsheet-map/#user-group) 
1. [What user groups use which applications?](/landscape/application-landscape-reports)
    1. Who is impacted when an application fails? 
1. [Where are users of applications located?](/location/application-usage-report)
    
<!--    
1. [Who uses which applications to provide a business capability?](/matrix/application-matrix-reports/#business-capability-user-group)
1. [Who uses which applications within a process?](/matrix/application-matrix-reports/#process-user-group)
1. [How will user groups use of applications change over time?](/matrix/application-matrix-reports/#time-user-group)
-->


## Business Capabilities

1. [What business capabilities do we have?](/inventory) 
1. [What business capabilities support our business?](/factsheet-map/#business-capability)
1. [Which business capabilities are supported by applications?](/landscape/application-landscape-reports)
    1. Which business capabilities are impacted when an application fails? 
1. [What is the IT cost of supporting a business capability?](/cost/business-capability-cost-report)

## Processes

1. [What Processes do we have?](/inventory)
1. [Who are the stakeholders involved in each process?](/inventory)
1. [How are our processes organised?](/factsheet-map/#user-group)
1. [What processes are supported by which applications?](/landscape/application-landscape-reports)
    1. What processes are impacted when an application fails?
1. [Which applications support a business process?](/landscape/application-landscape-reports)

## Applications

1. [What applications do we have?](/inventory)
1. [Who are the stakeholders involved in each application?](/inventory)
1. [What applications support which user groups?](/landscape/application-landscape-reports)
1. [What applications support which business capabilities?](/landscape/application-landscape-reports)
    1. Can applications supporting the same business capability be rationalised?
1. [What applications support which processes?](/landscape/application-landscape-reports)
1. [What applications are at risk due to obsolescent underlying IT components?](/matrix/application-matrix-reports/) 
1. [What applications are changed or impacted by which projects?]() - free draw, project roadmap with applications as children
1. [What applications are used by a user group to support a business capability?](/matrix/application-matrix-reports/#business-capability-user-group)
1. [What applications are used by a user group to perform a process?](/matrix/application-matrix-reports/#process-user-group)
1. [What applications are used to support a business capability used to perform a process?](/matrix/application-matrix-reports/#process-user-group)
1. For a group of related functions, what applications implement these, what is there status and roadmap? 
1. [What is the application roadmap?](/roadmap/application-roadmap-reports)
1. For a group of related functions, what is the overall driver for change, intent and roadmap? 
1. For applications implementing a group of related functions, what is the target application, roadmap, and what is the status of the roadmap plan? 
1. What is the health of applications and what action is required? (TIME: Tolerate, Invest, Migrate, Enhance) based on functional and technical fitness survey and other inputs. 
1. In which applications should we invest, which divest?
1. How does the application portfolio change over time (planned and proposed)? 
1. Is the application portfolio evolution aligned to strategic business priorities?
1. Does an application process any sensitive data, how is this data classified, where is it located? 
1. What is our cost structure?
1. [What is the IT cost of operating an application?](/cost/provider-cost-report)
1. [How many applications are active or being phased out?](/metrics/lifecycle-and-age-report)
1. [How many applications became active each year?](/metrics/lifecycle-and-age-report)
1. What applications are critical to support which business capabilities?
1. What changes have occurred in the application portfolio since the last reporting period? 
    1. applications added, retired, change in status, renamed, change in roadmap dates, change in intent, etc.
    1. resource classification change
    1. lifecycle date changes (new Active, new Phase-out, End-of-life)
1. Where are applications used?^4^    
    

## Data

1. [What Data objects do we have?](/inventory), what is their data classification and who manages them? 
1. [What is the data objects do we manage](/factsheet-map/#data-object) and what is their data classification?
1. [Where is sensitive data stored? Is there a sovereignty risk?](location/it-component-location-report) - *Filter by Data Classification.*
1. [What applications perform operations (CRUD) on data objects?](https://store.leanix.net/en/report-details/753b11a9-4e86-4fad-a840-f76341bad983/c7d772df-2988-4024-920f-fb732d95cedc) - *Custom report* 
1. [What applications manage sensitive data?](https://store.leanix.net/en/report-details/753b11a9-4e86-4fad-a840-f76341bad983/c7d772df-2988-4024-920f-fb732d95cedc) - *Custom report* or use [application matrix report](/matrix/application-matrix-reports) with data classification view
1. [What Applications providers and consume data via interfaces?](interface/interface-circle-map-report)
1. [How is sensitive data transferred through the IT landscape?](interface/data-flow-diagram)

## Interfaces

1. [What Interfaces do we have?](/inventory) 
1. [What data flows between applications?](interface/interface-circle-map-report/) 
1. [How does data flow through the IT landscape?](/interface/data-flow-diagram/)
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
1. [Is the project budget on track?](/cost/project-cost-report/)
1. [When will a project be completed?](/roadmap/project-roadmap-reports)
1. [Which projects provide the highest value at the lowest risk?](/metrics/project-portfolio-report)

## IT Components

1. [What IT Components do we have](/inventory), what are their properties, and who manages them? 
1. [Where are IT Components located?](location/it-component-location-report)
1. What technology implements an application? IT Component matrix with Application children or data flow or free draw
1. [How is the technology portfolio planned to evolve year by year?](/matrix/it-component-matrix-reports/#time-technical-stack) 
    1. [What is the technology roadmap?](/roadmap/project-roadmap-reports)
    1. What projects are implementing the technology roadmap?
1. What are our technical standards (preferred product to perform a function)? IT Component landscape with resource classification view - not answering functional bit. Need resource classification between application and business capability
  1. Which are standard technologies and can we reuse a solution?
1. [Is there opportunity to consolidate technologies?](/landscape/it-component-landscape/) 
1. How is an application hosted and how is this planned to evolve?


## Technical Stack

1. [What technology categories do we use?](/inventory)
1. [How are technology categories organised in a hierarchy to help classify IT components?](/factsheet-map/#technical-stack)
1. [What are our preferred IT components to use in a technology category?](/landscape/it-component-landscape/) 


## Providers

1. [What provider do we use?](/inventory)
1. Who is the provider of an application / technology? 
1. What is the aggregate risk around a provider?
1. Is there an opportunity to reduce the number of providers we deal with by changing technologies](/matrix/it-component-matrix-reports/#technical-stack-provider)
1. [What is the aggregate IT spend by provider?](../cost/provider-cost-report/) 
1. [Which provider relationships need closer management?](/metrics/provider-portfolio-report)

<!--

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

1. nsights into whether an Application and the Business Capability it supports are at risk is therefore derived from the underlying IT Components.
1. How many IT Components are redundant?
1. Which Applications are at risk as the underlying IT components are out of the lifecycle?
1. Which IT Components go Out-of-Life?
1. Which Countries are most affected by Tech Risk?
1. Which actions are planned to mitigate the risk by the individual Application owners?

BTM

1. 

-->

<!-- Links -->

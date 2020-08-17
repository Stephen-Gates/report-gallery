---
Title: "Questions you can answer with LeanIX reports"
---

??? note "Work in progress"
    This list needed to be rationalised and link to report pages.
    Take inspiration from the How to Answer the [Top Questions of Enterprise Architecture Stakeholders](https://www.leanix.net/en/download/how-to-answer-the-top-questions-of-enterprise-architecture-stakeholders) poster."

# Questions you can answer with LeanIX reports

## User Groups

1. [What User Groups are part of, or interact with, our business?](factsheet-map-reports/user-group-factsheet-map-report.md)
1. Who uses applications?

## Business Capabilities

1. Which applications support which business capability?
1. Which applications need to improve to met the desired business capability maturity level?
1. [What is the IT spend by business capability?](cost-analysis-reports/business-capability-cost-report.md)

## Processes

1. What processes are impacted when an application fails?
1. Which applications support a business process?
1. What does the process workflow look like at various steps?
1. Who are the stakeholders involved in each process?

## Applications

1. What applications do we have? 
1. What functions do applications perform? 
1. Do we have applications that perform the same function that should be considered for consolidation? 
1. What changes have occurred in the application portfolio since the last reporting period? 
    1. applications added, retired, change in status, renamed, change in roadmap dates, change in intent, etc.
    1. resource classification change
    1. lifecycle date changes (new Active, new Phase-out, End-of-life)
1. For a group of related functions, what applications implement these, what is there status and roadmap? 
1. For a group of related functions, what is the overall driver for change, intent and roadmap? 
1. For applications implementing a group of related functions, what is the target application, roadmap, and what is the status of the roadmap plan? 
1. What is the health of applications and what action is required? (TIME: Tolerate, Invest, Migrate, Enhance) based on functional and technical fitness survey and other inputs. 
1. Who is using applications. Where are these users located?
1. How does the application portfolio change over time (planned and proposed)? 
1. Is the application portfolio evolution aligned to strategic business priorities?
1. Who are the technical and business owners of an application? 
1. What applications are owned by a particular person / role / organisation unit? 
1. Does an application process any sensitive data, how is this data classified, where is it located? 
1. What is the application roadmap?
1. In which applications should we invest, which devest?
1. What is our cost structure?
1. Where do we face risks through technology obsolescence?

## Data

1. [What data objects do we manage?](factsheet-map-reports/data-object-factsheet-map-report.md)
1. [What is the data classification of a data object?](factsheet-map-reports/data-object-factsheet-map-report.md) - *use Data Classification view*
1. [Where is sensitive data stored? Is there a sovereignty risk?](location-reports/it-component-location-report.md) - *Filter by Data Classification.*
1. Who is in data governance roles for a data object? - *inventory report*
1. [What applications perform operations (CRUD) on data objects?](https://store.leanix.net/en/report-details/753b11a9-4e86-4fad-a840-f76341bad983/c7d772df-2988-4024-920f-fb732d95cedc) - *Custom report* 
1. [What applications manage sensitive data?](metrix-reports/application-portfolio-reports) - *use Data Classification view*
1. [What Applications providers and consume data via interfaces?](interface-reports/interface-circle-map-report.md)
1. [How is sensitive data transferred through the IT landscape?](interface-reports/data-flow-diagram.md)

## Interfaces

1. What data flows between applications? 
1. How does sensitive data flow through the IT landscape?
1. How is it transported (SFTP, API)
1.  What is the frequency of the data flow (real-time, hourly, etc.
1. How are interfaces connecting the IT landscape?
1.  What application integrations exist across the IT landscape? (See: [Interface Circle Map Reports](doc:interface-circle-map-reports))  

## Projects 

1. What applications are impacted by which projects? 
1.  What initiative plan to change the application portfolio?
1. Are any technology elements missing that are needed to support the proposed project portfolio?
1. What budget is planned for certain projects?
1. When will the project for consolidating customer platform be completed?
1. Is the project budget on track?
1. Which projects provide the highest value at the lowest risk?

## IT Components

1. What technology implements an application? 
1. Which applications are at risk due to legacy technology (provider end of support, end of life dates)? 
1. How is the technology portfolio evolving over time? 
1.  What are our technical standards (preferred product to perform a function)? 
1. Is there opportunity to consolidate technologies? 
1. How is an application hosted and how is this planned to evolve?
1. What is the technology roadmap?
1. Which are standard technologies and can we reuse a solution?

## Providers

1.  Who is the provider of an application / technology? 
1. What is the aggregate risk around a provider?
1.  Is there an opportunity to reduce the number of providers we deal with by changing technologies / applications
1. What is the IT spend by provider? 

## Technology Stack

1. What categories / hierarchy is used to describe the technology stack
1. What technologies do we have in a technology category
1. Is there opportunity to consolidate technologies? 

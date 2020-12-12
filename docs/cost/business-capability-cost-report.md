---
title: "Business Capability Cost report"
---

# Business Capability Cost report
## Overview

The Business Capability Cost report answers the question:

>What is the IT spend by business capability?

The costs for a Business Capability are calculated based on:

- the Applications that support the Business Capability
- the aggregate annual costs of the IT Components that implement the Application
- filtered by an Application Lifecycle that is effective within time frame or at a point of time
- filtered by any other constraints to focus on the area of interest 

![Business Capability Cost report](../assets/images/cost-business-capability.png)

*Business Capability Cost report for Applications with Any Lifecycle value effective within the 2020 timeframe.*

## Requirements

### Factsheets

The following factsheets and associated properties are required:

- Business Capability
    - related to one or more Applications
- Application
    - related to one or more IT Components
- IT Component
    - Annual cost on Application - IT Component relationship

For more information, check the [report requirements in the LeanIX User Docs](https://docs.leanix.net/docs/report-overview).  

### Other requirements

Overlapping dates on relationships and report date filter.
<!-- See https://docs.leanix.net/docs/insights-through-reports#knowledge-about--relations-in-eg-application-landscape -->

## Settings

Display this report as a chart or table. The table view cannot show the annual costs as they are stored on the Application - IT Component relationship.

![Business Capability Cost table](/assets/images/cost-business-capability-table.png)

*Business Capability Cost table.*


## Filters

[Use filters][report-filters] to focus on the required Business Capabilities

<!-- other links -->

[report-filters]: https://docs.leanix.net/docs/searching-and-filtering-functions-in-leanix#searching-in-reports

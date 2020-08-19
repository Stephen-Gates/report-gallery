---
title: "Provider Cost report"
---

??? note "Work in progress"
    - how are costs calculated IT Components & Projects? 
    - need image

# Provider Cost report
## Overview

The Provider Cost report answers the question:

***[What is the IT spend by Provider?](../questions.md#costs)***

The costs for a Provider are calculated based on:

- ~~the Applications that support the Provider~~
- ~~the aggregate annual costs of the IT Components that implement the Application~~
- ~~filtered by an Application Lifecycle that is effective within time frame or at a point of time~~
- ~~filtered by any other constraints to focus on the area of interest~~

![Provider Cost report](/assets/images/cost-analysis-report-bc.png)

*Provider Cost report for Applications with Any Lifecycle value effective within the 2020 timeframe*

## Requirements

### Factsheets

The following factsheets and associated properties are required:

- Provider
    - related to one or more Applications
- Application
    - related to one or more IT Components
- IT Component
    - Annual cost on Application - IT Component relationship
- Project?

For more information, check the [report requirements in the LeanIX User Docs](https://docs.leanix.net/docs/report-overview) 

### Tags 

No tags are required for this report.

### Other requirement

Overlapping dates on relationships and report date filter.
<!-- See https://docs.leanix.net/docs/insights-through-reports#knowledge-about--relations-in-eg-application-landscape -->

## Settings

This report may be displayed as a chart or a table. The table view cannot show the costs as they are stored on the Provider relationships.

## View

This report has no views.

## Filters

Filters can be used to focus on the required Providers

## Editing

This report cannot be edited.

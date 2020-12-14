---
title: "Application Matrix reports"
---

??? note "Work in progress"
    - Add ==questions==
    - Add use cases

# Application Matrix reports

## Overview

Application Matrix report shows Applications within a matrix of:

- on the horizontal axis: Business Capabilities, Processes, or Time Frame
- on the vertical axis: Business Capabilities, or User Groups

![Application Matrix report](../assets/images/application-matrix-bc-ug.png)  

<p id="caption">Application Matrix report, Business Capability × User Group, Business Criticality view.</p>

There are five Application Matrix reports: 

1. [Business Capability × User Group](#business-capability-user-group) - ==question==
1. [Process × Business Capability](#process-business-capability) - ==question==
1. [Process × User Group](#process-user-group) - ==question==
1. [Time × Business Capability](#time-business-capability) - ==question==
1. [Time × User Group](#time-user-group) - ==question==

Each report has different data requirements and is configured using different settings.

All reports have the same views, filters, and can be edited. 

### Views

The views available are:

#### Fields on the factsheet 

1. [Lifecycle][lifecycle-view]
1. [Application Functional Fit][application-functional-fit-view]
1. [Application Technical Fit][application-technical-fit-view]
1. [Application Business Criticality][application-business-criticality-view]

#### Fields on relations

1. [IT Components: Total annual cost][application-total-annual-cost-view]

#### Fields on related factsheets

1. [Aggregated Obsolescence Risk][aggregated-obsolescence-risk-view]
1. [Data Classification][data-classification-view]
1. [IT Component Technical Fit][application-technical-fit-view]
1. [Project Risk][project-risk-view]
1. [Project Status][project-status-view]
1. [Project Business Value][project-business-value-view]

#### Tags

You can colour factsheets based on tags. [Tag colors](https://docs.leanix.net/docs/maintain-your-tags) are defined by your LeanIX Administrator.

### Filters

[Use filters][report-filters] to focus on the required factsheets.

### Editing

This report can be edited.

--- 

## Business Capability × User Group

The **Application Matrix - Business Capability × User Group report** answers the question:

> ==What is the question?==

This is useful specifically for... 

![Application Matrix report](/assets/images/application-matrix-bc-ug.png)  

<p id="caption">Caption.</p>

### Requirements

The following factsheets and associated properties are required:

- **Application**
    - lifecycle dates
    - relationship to Business Capability
    - relationship to User Group
- **Business Capabilities**
- **User Groups**

Other factsheet types may be required to support the drilldown feature. 

### Settings

- Horizontal Axis: **Business Capabilities**
- Hide empty columns: check or uncheck
- Vertical Axis: **User Group**
- Hide empty rows: check or uncheck
- Drilldown relation: 
    - \-  *(no drilldown is shown)*
    - Business Capabilities
    - Chlidren
    - Consumed Interfaces
    - Data Objects
    - IT Components
    - Parents
    - Predecessors
    - Processes
    - Projects
    - Provided Interfaces
    - Required by
    - Requirements
    - Successors
    - User Groups

--- 

## Process × Business Capability 

The **Application Matrix - Process × Business Capability report** answers the question:

> ==What is the question?==

This is useful specifically for... 

![Application Matrix report](/assets/images/application-matrix-process-bc.png)  

<p id="caption">Caption.</p>

### Requirements

The following factsheets and associated properties are required:

- **Application**
    - lifecycle dates
    - relationship to Process
    - relationship to Business Capability
- **Business Capabilities**
- **Process**

Other factsheet types may be required to support the drilldown feature. 

### Settings

- Horizontal Axis: **Processes**
- Hide empty columns: check or uncheck
- Vertical Axis: **Business Capabilities**
- Hide empty rows: check or uncheck
- Drilldown relation: 
    - \-  *(no drilldown is shown)*
    - Business Capabilities
    - Chlidren
    - Consumed Interfaces
    - Data Objects
    - IT Components
    - Parents
    - Predecessors
    - Processes
    - Projects
    - Provided Interfaces
    - Required by
    - Requirements
    - Successors
    - User Groups

--- 

## Process × User Group

The **Application Matrix - Process × User Group report** answers the question:

> ==What is the question?==

This is useful specifically for... 

![Application Matrix report](/assets/images/application-matrix-process-ug.png)  

<p id="caption">Caption.</p>

### Requirements

The following factsheets and associated properties are required:

- **Application**
    - lifecycle dates
    - relationship to Process
    - relationship to User Group
- **Process**
- **User Group**

Other factsheet types may be required to support the drilldown feature. 

### Settings

- Horizontal Axis: **Processes**
- Hide empty columns: check or uncheck
- Vertical Axis: **User Groups**
- Hide empty rows: check or uncheck
- Drilldown relation: 
    - \-  *(no drilldown is shown)*
    - Business Capabilities
    - Chlidren
    - Consumed Interfaces
    - Data Objects
    - IT Components
    - Parents
    - Predecessors
    - Processes
    - Projects
    - Provided Interfaces
    - Required by
    - Requirements
    - Successors
    - User Groups

--- 

## Time × Business Capability 

The **Application Matrix - Time × Business Capability report** answers the question:

> ==What is the question?==

This is useful specifically for... 

![Application Matrix report](/assets/images/application-matrix-time-bc.png)  

<p id="caption">Caption.</p>

### Requirements

The following factsheets and associated properties are required:

- **Application**
    - lifecycle dates
    - relationship to Business Capability
- **Business Capability**

Other factsheet types may be required to support the drilldown feature. 

### Settings

- Horizontal Axis: **Time Frame**
- Hide empty columns: **uncheck** (check doesn't make sense when Time Frame is the axis)
- Vertical Axis: **Business Capabilities**
- Hide empty rows: check or uncheck
- Drilldown relation: 
    - \-  *(no drilldown is shown)*
    - Business Capabilities
    - Chlidren
    - Consumed Interfaces
    - Data Objects
    - IT Components
    - Parents
    - Predecessors
    - Processes
    - Projects
    - Provided Interfaces
    - Required by
    - Requirements
    - Successors
    - User Groups
    
--- 

## Time × User Group

The **Application Matrix - Time × User Group report** answers the question:

> What is the question?

This is useful specifically for... 

![Application Matrix report](/assets/images/application-matrix-time-ug.png)  

<p id="caption">Caption.</p>

### Requirements

The following factsheets and associated properties are required:

- **Application**
    - lifecycle dates
    - relationship to User Groups
- **User Group**

Other factsheet types may be required to support the drilldown feature. 

### Settings

- Horizontal Axis: **Time Frame**
- Hide empty columns: **uncheck** (check doesn't make sense when Time Frame is the axis)
- Vertical Axis: **User Groups**
- Hide empty rows: check or uncheck
- Drilldown relation: 
    - \-  *(no drilldown is shown)*
    - Business Capabilities
    - Chlidren
    - Consumed Interfaces
    - Data Objects
    - IT Components
    - Parents
    - Predecessors
    - Processes
    - Projects
    - Provided Interfaces
    - Required by
    - Requirements
    - Successors
    - User Groups
 

<!-- view links -->

[lifecycle-view]: https://docs.leanix.net/docs/reporting-views#1-lifecycle
[application-functional-fit-view]: https://docs.leanix.net/docs/reporting-views#2-functional-fit
[application-technical-fit-view]: https://docs.leanix.net/docs/reporting-views#3-technical-fit
[it-component-technical-fit]: https://docs.leanix.net/docs/reporting-views#3-technical-fit
[application-business-criticality-view]: https://docs.leanix.net/docs/reporting-views#4-business-criticality
[aggregated-obsolescence-risk-view]: https://docs.leanix.net/docs/reporting-views#5-technology-risk
[project-risk-view]: https://docs.leanix.net/docs/reporting-views#6-project-risk
[project-status-view]: https://docs.leanix.net/docs/reporting-views#7-project-status
[project-cost-view]: https://docs.leanix.net/docs/reporting-views#8-project-business-value-budget-opex--capex
[project-business-value-view]: https://docs.leanix.net/docs/reporting-views#9-project-business-value-npv
[provider-quality-view]: https://docs.leanix.net/docs/reporting-views#10-provider-quality
[provider-criticality-view]: https://docs.leanix.net/docs/reporting-views#11-provider-criticality
[application-total-annual-cost-view]: https://docs.leanix.net/docs/reporting-views#12-it-componentsapplications-total-annual-cost
[it-component-resource-classification]: https://docs.leanix.net/docs/reporting-views#13-technical-stacksit-components-resource-classification
[data-classification-view]: https://docs.leanix.net/docs/reporting-views#14-data-object-application-data-classification

<!-- other links -->

[report-filters]: https://docs.leanix.net/docs/searching-and-filtering-functions-in-leanix#searching-in-reports

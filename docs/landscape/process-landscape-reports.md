---
title: "Process Landscape reports"
---

??? note "Work in progress"
    - Report in development by LeanIX

# Process Landscape report

## Overview

The Process Landscape report answers the questions:

>- What Processes use Business Capabilities?
>- What Processes are used by  Processes?
>- What Processes are used by  User Groups?

There are three Process Landscape reports that show the Process Landscape, within a hierarchy of:

- Applications 
- [Business Capabilities](#business-capability)
- [Processes](#process)
- [User Groups](#user-group)


![Application Landscape report](../assets/images/application-landscape.png){: .zoom }

<!--
![](https://www.leanix.net/hubfs/2019%20LX%20Website/General/Illu/techrisk-drilldown-7-Col-XL.svg)
-->


*Application Landscape for Business Capabilities, Business Criticality view.*

--- 

## Business Capability

This report answers the question:

- *[What Applications support Business Capabilities?](../questions/#business-capability)*

This is useful for... 

![Application Landscape report](../assets/images/application-landscape-bc-criticality.png){: .zoom }

*Caption.*

### Requirements

#### Factsheets

Specific factsheets and associated properties are required:

- Business Capability 
- Process
    - Process - Business Capability requires relationship
    
#### Tags 

Specific tags are required for this report.

#### Other requirement

No other requirements

### Settings

Specific settings for this report 

### View

Specific view available are: 

### Filters

Use filters to focus on the required Business Capabilities.

--- 

## Process
This report answers the question:

- *[What Applications support Process?](../questions/#process)*

This is useful specifically for... 

![Application Landscape report](../assets/images/application-landscape-process-lifecycle.png){: .zoom }

*Caption.*

### Requirements

#### Factsheets

Specific factsheets and associated properties are required:

- Process 
- Application
    - Application - Process relationship
    
#### Tags 

Specific tags are required for this report.

#### Other requirement

No other requirements

### Settings

Specific settings for this report 

### View

Specific view available are: 

### Filters

Use filters to focus on the required Processes.

--- 

## User Group 

This report answers the question:

- *[What Applications support User Groups?](../questions/#user-groups)*

This is useful specifically for... 

![Application Landscape report](../assets/images/application-landscape-ug-lifecycle.png){: .zoom }

*Caption.*

### Requirements

#### Factsheets

Specific factsheets and associated properties are required:

- User Group 
- Application
    - Application - User Group relationship

#### Tags 

Specific tags are required for this report.

#### Other requirement

No other requirements

### Settings

Specific settings for this report 

### View

Specific view available are: 

### Filters

Use filters to focus on the required User Groups.

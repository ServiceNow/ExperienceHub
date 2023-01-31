---
title: Selecting a Canvas
share-description: At the start of a project building an application on ServiceNow, you need to make decisions about what interface(s)to use for the user groups. Which interface(s) provide the right experience for the users’ skills, their frequency of use, and the amount of data presented to them. 
layout: page
permalink: /guides/selecting-a-canvas
---
Unlike other platforms, or bespoke applications, ServiceNow provides multiple user interfaces designed for different personas. Each option is ideal for specific use cases and users and your choices impact the experience perceived by your users.

## Preparations for choosing a canvas
* Define the use cases your application solves for
* Conduct [user research](methods/user-interviews) to understand your users’ skill levels and mental models

## Questions to consider
* Have you defined the user personas that interact with your application?
* How frequently will your personas interact with your application? Can they become experts?
* Will you provide training to your users?
* What development skills do you have access to?

## The Canvases
Within the NOW Platform there are currently 4 different canvases to choose from when delivering an app. A customer’s current release and licensing impact the availability of these canvases on your instance.

### Classic Environment

|Topic  | Description|
| ----- | ----------- |
|**Target Use Case(s)**|Administering the platform or an application built on the platform|
|**Builder Tools**|CoreUI – Dashboard Builder, Theme Editor|
|**Target Users**|Platform Admins and Owners, Application Admins|

The Classic Environment is ServiceNow’s user interface best tailored for administering the instance or applications you build on the platform.

 

Administrators of your instances configure unique views of lists and tables for specific users, groups, and roles. Depending on an individual user’s permissions, they may also be able to create their own unique views of lists & forms.

With the San Diego release a new application shell for the Classic Environment is now available. Called Next Experience, this optional change provides an intuitive, personalized experience to drive productivity and engagement. This replaces the CoreUI (aka UI16, Classic UI, List and Forms)
 


#### Key Features

|Core UI| Next Experience|Notes|
| ------- | --------------- | ----- |
|Homepages and Dashboard|Landing Pages|	First thing a user sees when logging into the interface. Tailored to orient a user to their work at a glance determine where to start|
|Application Navigator|	Unified Navigation|	Allow a user to explore the applications and modules they have access to.|
|Notifications|	Notifications|	View and personalize notifications applicable to you based on access and admin configurations.|
|Search|	Global Search|	Search across your instance to return the results that are most relevant to you.|
|User Menu|	User Menu|	Personalize your instance and set your user preferences.«
|Help|	Help|Access on-demand help when you need it.


#### Customer Use Cases
1.	Your admins want to view all employees with their office location and then filter the view based on the location’s country.
    1.	You create a list layout view with the employee’s first name, last name, and location.
    1.	Your colleagues then can use the Search capabilities to find all employees at a specific office.
2.	Your platform owner asks to create a new landing page for them to show the status of all projects, requests, and cases on the instance to help them understand how ServiceNow is supporting the organization.
    1. Based on the requirements of your platform owner, determine whether you need to create a dashboard or landing page.
    1.	This new destination can be assigned specifically to the user, or a role or group assigned to them.

#### Target User Groups
The primary personas for this are your platform or application administrators that need to directly modify data or review data regarding those applications. Tailored to technical audiences, the Classic Experience is best for those is familiar with the ServiceNow platform. It is not appropriate for infrequent, non-expert, or non-technical users.

### Service Portal

|Topic  | Description|
| ----- | ----------- |
|**Target Use Case(s)**|Self-service experiences for getting help, requesting things, and consuming content|
|**Builder Tools**|Service Portal Page Design, Branding Editor, Widget Editor|
|**Target Users**|External customers, employees in need of support to resolve issues|

The Service Portal framework is primary user interface for users requesting items from service catalogs and consuming content from knowledge bases. You can use Service Portal Designer and related tools to configure pages, themes, widgets and customize entire web applications in the tools. Service Portal uses common, open-source web technologies including AngularJS, Bootstrap v3, and SASS so it is a welcome platform for modern web developers.

Also, many of ServiceNow’s core products use the framework to build the out of the box portals for their offerings. This includes Employee Center, Customer Service Portal, and Consumer Service Portal

A portal consists of pages made up of widgets. ServiceNow provides widgets out of the box with various products, there are partners that sell widget libraries, and customers can build their own.

The Service Portal Branding Editor provides a simplified interface for setting basic styles (CSS properties) in an intuitive interface. The editor allows customers to override the default styles specified by Bootstrap and any out of the box overrides. 

For fine-grained control of styles, customers can:
* Create themes to apply to many portals
* Define page specific styles
* Define widget specific styles
* Override styles within an instance of a widget

To learn more about Service Portal capabilities, check out [Understanding Service Portal](https://docs.servicenow.com/bundle/sandiego-servicenow-platform/page/build/service-portal/concept/sp-what-to-know.html) on our Product Docs site.

#### Customer Use Cases

1. Imagine you already implemented Employee Center  and recently built an app to manage complimentary employee car washes
    1. Create a widget to the existing portal that shows if they have car wash credits available, upcoming appointments, and a button to schedule an appointment
    1. Create a standalone app using App Engine Studio to schedule appointments and manage the car wash data
1. You built a complex application to manage market-specific promotions for products. Various end users may have the ability to view, create, approve those promotions
    1. Create a standalone portal focused on the Market Promotions applications. This will used permissions to manage what users can see and do.
    1. If the customer has an existing Employee Center portal, there are ways to push tasks and approvals from the app into the view. This will ensure actions are not siloed into the dedicated portal.

***
Service Portals can manage user access to content using a capability called User Criteria. This allows a single portal to serve diverse roles through access control of:

* Pages
* Widgets & Instances
* Announcements
* Catalog items
* Knowledge Articles & Knowledge Blocks
* Search Sources

***

#### Target User Groups
The primary personas for this are users that are seeking help or the ability to self-service issues they may encounter during their day. These “requestor” personas are infrequent users with limited experience with the ServiceNow platform and need an intuitive, low learning curve experience so they can get back to work. Service Portal is not meant to be a primary work interface for users. 

### Configurable Workspaces 

|Topic  | Description|
 --- | ---|
|**Target Use Case(s)**|Resolving problems created by requestors|
|**Builder Tools**|UI Builder, ServiceNow CLI|
|**Target Users**|Agents, case managers, service desk professionals, and managers|

Configurable Workspaces meet the needs of users handling cases, tickets, incidents, or other request types on a regular basis. The capabilities of Configurable Workspace support the needs of these personas to collaborate with colleagues, answer customer questions, and resolve their problems. Consider workspaces the “command center” for your service-focused employees.

The Next Experience powers Configurable Workspaces allowing them to nicely integrate into the Unified Navigation of the Classic Environment. This provides a consistent look and feel across the platform for users that span the different canvases. 

Many of ServiceNow’s out of the box products leverage Configurable Workspaces for their relevant use cases, providing a starting point for your specific project needs. Make sure to check the products you own and the Workspaces your colleagues already use.

To create workspace experience that meet the needs of your project, UI Builder is ServiceNow’s page builder where you create new pages, configure existing pages, and leverage Next Experience components or your own custom web components.
 
***
UI Builder supports more than just custom workspaces; it allows you build other types of pages. Learn More about UI Builder on Community

***

#### Customer Use Cases
1.	Your project expects users to review PDF documents daily, annotating the documents with copy changes and requests for new illustrations. These users process multiple documents a day and it is their primary work activity.
    1. Add a button to a record page, allowing users to open the PDF for review in a new workspace page.
    1. Create a new page in UI Builder that uses Adobe’s PDF Embed API to embed the relevant document in the browser, capturing annotations as the user leaves them.
2.	Your team is building a workspace for foster care placements. In each placement record, your users need to see the household members living with the foster child.
    1. Add a custom component to the contextual side panel listing all family members with a photo, name, and relation (foster parent, sibling, etc.)
    1. When a user clicks on a person’s card, open a new tab showing the record with additional data about the household member.

#### Target User Groups
Configurable Workspaces meet the needs of agents, case managers, service desk professionals, and managers as an interface focused on supporting the resolution of customer problems. Those customers include external customers as well as internal employees encountering problems that disrupt their workday. These users are a captive audience, trained for their case management role and spending most of their workday interacting with this solution.


### Native Mobile
ServiceNow offers two native mobile applications for iOS and Android that provide your creators the ability to leverage mobile devices unique capabilities in their applications.

#### Now Mobile

|Topic  | Description|
 --- | ---|
|**Target Use Case(s)**|Self-service experiences for getting help, requesting things, and consuming content|
|**Builder Tools**|Mobile App Builder, Mobile Card Builder, Mobile Studio|
|**Target Users**|Employees in need of support to resolve issues, manage tasks, and access company resources|

For most employees, the Now Mobile app is the primary native mobile experience tailored to them. This app experience is ideal for short, transactional interactions focused on finding answers to problems, requesting something, or approving others’ requests

### Mobile Agent

|Topic  | Description|
 --- | ---|
|**Target Use Case(s)**|Allow agents to triage, address and resolve requests|
|**Builder Tools**|Mobile App Builder, Mobile Card Builder, Mobile Studio|
|**Target Users**|Service agents and field agents that are not in a fixed location.|

For service agents or fields agents the Mobile Agent app is the primary native mobile experience tailored to their unique needs. Agents can get work done anywhere through an easy to navigate native mobile interface.

***
**Note** With the Rome Release in 2021, ServiceNow deprecated the separate Mobile Onboarding app. The NOW Support app’s primary persona is the Instance Administrator responsible for managing the ServiceNow environment.
***

## Where to go next
Once you decide which interface(s) to use for your application it is time to decide how to configure and/or customize them. To learn more about the interfaces, see the content below

[Classic Environment – CoreUI](https://docs.servicenow.com/csh?topicname=c_UI16.html&version=latest)

[Classic Environment– Next Experience](https://docs.servicenow.com/csh?topicname=next-experience-landing-page.html&version=latest)

[Service Portal](https://docs.servicenow.com/csh?topicname=c_ServicePortal.html&version=latest)	 

[Native Mobile](https://docs.servicenow.com/csh?topicname=sg-setup-mobile-admin.html&version=latest) 

***
The Next Experience UI framework is constantly evolving. To stay up to date, follow progress in the [Next Experience Community](https://www.servicenow.com/community/next-experience/ct-p/next-experience)
***
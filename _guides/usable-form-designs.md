---
title: Usable Form Design
share-description: Most applications built by ServiceNow or on the ServiceNow platform relies on the creation of data to power the workflows that deliver value to the business. Often, that data is created by human input through forms. To ensure desirable outcomes for the business and users, forms need to ask clear questions, use the simplest input to efficient collect data, and help the user recover when things go wrong. 
layout: page
permalink: /guides/form-design
---
## Introduction
Most applications built by ServiceNow or on the ServiceNow platform relies on the creation of data to power the workflows that deliver value to the business. Often, that data is created by human input through forms. To ensure desirable outcomes for the business and users, forms need to ask clear questions, use the simplest input to efficient collect data, and help the user recover when things go wrong. 
 
In short, forms need to be designed to reflect the user’s mental model of the data, not the systems.  
 
## Where do users encounter forms 
On the ServiceNow platform, there are 3 types of forms a user might encounter. 
1.	[Standard catalog item](https://docs.servicenow.com/csh?topicname=c_IntroductionToCatalogItems.html&version=latest) – presents a form to users that want to request a service or good and provide information about that request. This form uses Variables to define the fields presented. 
2.	[Record Producer](https://docs.servicenow.com/csh?topicname=c_RecordProducer.html&version=latest) – presents a form to users where the information they provide generates a task-based record (e.g., incident, case). This form uses Variables to define the fields presented. 
3.	[Form](https://docs.servicenow.com/csh?topicname=now-platform-forms-fields-lists.html&version=latest) – every table created on ServiceNow has a form automatically generated to allow for input of data into the table. Users can configure that form or add additional form views. This form type is typically encountered by administrative or fulfiller users. The fields presented in these forms are defined by the field types specified in the table definition. 
 
**Note**: [Order Guides](https://docs.servicenow.com/csh?topicname=c_ServiceCatalogOrderGuides.html&version=latest) are a variant of a Standard Catalog Item that allow a user to request multiple catalog items in a single request. The same input capabilities exist here as an Standard Catalog Item 
 
In ServiceNow, forms can be displayed in any of our user interfaces: 
-	Admins, working in the Core UI might use a form to create a new user. (Form View) 
-	Call center agents might log interaction details in a workspace. (Form View)  
-	Field technicians might enter diagnostic information in the mobile app (Form View) 
-	Employees may open a case with HR in Employee Center (Record Producer) 
-	A customer might request a service via the Service Catalog (Standard Catalog Item) 
 
Each of these UIs may be submitting data to the same tables but present a different form based on the user’s needs and environment. This is accomplished through Form Views. 
 
## Preparing to design 
When creating form views for your project, it is important have a clear understanding of the data the form needs to collect, the user persona(s) that will interact with the form, and the process that the form supports. It is also beneficial to know what data the system has available that can mitigate the need for user entry. 
 
## Understanding the data 
First, understand what data must be collected from the user. The emphasis is on must because it is important to consider what information the system already has, could have, or could access via an integration. For example, when working with a user logged into your system, you should not need to ask them to enter their name, email, or other information that already exists. It just adds to the effort to complete the form.  
 
Also, consider what the minimum amount of information needed to collect from the user. Can some data be generated automatically based on other inputs? Can the system or fulfiller fill in gaps in the data through automation or developed expertise?  
 
## Understand the process 
To design a good form and ensure you are asking the right questions at the right time, it helps to understand the process the form supports. What does the system or recipient of the form data do with the information once it is received? If another person interacts with the data, before the process is complete, what do they do with the data? Does the process require someone to talk to the user again before the process completes? 
 
It is important to understand this information as it may guide when a user is asked for information. Also, knowing how information is going to be used will help users provide more accurate information in their responses 
 
 
## Understanding the user persona(s) 
In form design, it is important to learn what information a user has when they encounter a form. Is it information that they can easily recall and enter, or does it require critical thinking, research, or analysis? If the user can’t easily recall the information, is the answer accessible to them in an available reference? 
 
As you approach defining the inputs in a form, spend time talking to your users to gain an understanding of their readiness and ability to answer the questions.  
 
## Go Further 
It helps to talk to your users before you design the form and when appropriate, conduct [usability testing](/methods/usability-testing) to validate the efficacy of your design.

Once you develop a solid understanding of your users, the process, and the data it is time to design the forms that will power the experience. Read Form Design Best Practices for guidance on the best way to apply your learnings.
 

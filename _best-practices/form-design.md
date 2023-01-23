---
title: Form Design Best Practices
share-description: The way a form is built impacts the quality of the data provided into the process. It is important to design forms that users can clearly comprehend, interact with, and get feedback from. This article presents specific guidelines on how to use the capabilities of ServiceNow’s forms and catalog items to follow the best practices.
layout: page
permalink: /best-practices/form-design
---
## Overview
The way a form is built impacts the quality of the data provided into the process. It is important to design forms that users can clearly comprehend, interact with, and get feedback from. This article presents specific guidelines on how to use the capabilities of ServiceNow’s forms and catalog items to follow the best practices. Please consider reading Getting Input: How to seamlessly get information from your users to develop an understanding the purpose of the forms you are creating.

## Principles
Once you understand the data you need, the process the data supports, and the knowledge and expectations of the user you can start to define the questions to ask and controls to use to collect that information. 
 
In the book [Web Form Design, Filling in the Blanks](), Luke Wroblewski defines 4 principles of good form design: 
* Minimize the pain 
* Illuminate a path to completion 
* Consider the context 
* Ensure consistent communication. 

How might you consider implementing forms (record producers, order guides, etc) on ServiceNow following these principles?

### Minimize the Pain 
This principal focus on the fact that “people want what lies on the other side of the form.” Each question that is added, increases the friction between a user and their goal. When designing the form, consider the value of each additional question asked versus the pain inflicted upon the user. 
 
The platform can help with this.  
 
Depending on how your organization is using ServiceNow the data may already exist on the platform. Can it be achieved via a lookup based on the logged in user or other data entered? 
 
ServiceNow also provides powerful integration capabilities via IntegrationHub. Is there another system – either external or internal – that can provide the data? 
 
Finally, consider if the user is the best person to answer the question. Maybe, the answer can be calculated by other data provided, generated via logic rules, or completed on the fulfillment side. 

### Illuminate a path to complete 
When a user looks at a form, the steps to complete and successfully submit should be clear.  At its most basic, users should know what fields are required versus optional.  
 
When configuring a form with ServiceNow, any field marked as mandatory in the table definitions will require user input before the form can be submitted. 
 
Another useful capability to identify the path, is to create sections to your form. This enables to form to logically group related fields into structured sections that a user can complete in progression. 
 
**Note:** Besides [Order Guides](https://docs.servicenow.com/csh?topicname=c_ServiceCatalogOrderGuides.html&version=latest), ServiceNow forms are always single page. There is not currently a multistep form experience supported out of the box. The [ServiceNow Community](https://www.servicenow.com/community/) may have some third-party examples. 

### Consider the Context 
Users typically encounter a form as part of a broader experience. Maybe they received an alert or saw a new incident pop up in a list. Perhaps they came to a portal because they encountered an issue in their day. 
 
Given these potential triggers, consider what support you can provide your user to complete this step more seamlessly.

### Ensure Consistent Communication 
A form serves as way for groups to communicate with their colleagues or customers. Any individual might encounter multiple forms during their relationship with a company. Consider the method of data collection and tone used across multiple forms. 
 
Establish Best Practices for form designs, that anyone who can create a form is required to follow. This should cover the types of fields to use for question types and standards for how to collect groups of information (e.g., addresses). See the section below for our guidance on form design. 
 
For [Catalog items](https://docs.servicenow.com/csh?topicname=c_IntroductionToCatalogItems.html&version=latest) and [Record Producers](https://docs.servicenow.com/csh?topicname=c_RecordProducer.html&version=latest), [Variable Sets](https://docs.servicenow.com/csh?topicname=c_ServiceCatalogVariableSets.html&version=latest) provide a block of pre-defined fields to reuse across the catalog. As an example, an administrator can define a specific way to collect an address from a user. This then can be used by any item in the catalog; ensuring consistency every time an address is requested. 

## Best Practices
Considering the principles we outlined, how might you best configure your forms to create efficiency and delight?

### Input Types
The type of data you need should guide the type of field or variable type used to collect that information. Here is a recommendation guide matching different input needs to the field types or variable types on the platform. 

There are two different sets of form controls in ServiceNow. One, **[Field Types](https://docs.servicenow.com/bundle/sandiego-platform-administration/page/administer/reference-pages/reference/r_FieldTypes.html)** are defined at the table-level and affect all form views of that table. **[Variable Types](https://docs.servicenow.com/bundle/sandiego-servicenow-platform/page/product/service-catalog-management/reference/r_VariableTypes.html#d257767e1556)** relate to the form controls used on service catalog items

| Data you want to collect | Field Type | Variable Type |
| ----------- | ----------- | ----------- |
|Binary response – Yes/No, True/False, On/Off|True/False|Yes/No|
|Selecting one item from a list (<6 items)|Choice|* Multiple Choice * Lookup multiple choice (if choices are from a table)|
|Selecting one item from a list (6+ items)|Choice|-  Select Box OR Lookup select box (if choices are from a table)|
|Selecting multiple items from a list (<6 items)|???|  Checkbox|
|Selecting multiple items from a list (6+ items)|???| List collector|
|Open ended questions (short)|String or String (Full UTF-8)*|Single-line text|
|Open ended questions (long)|String???|Multi-line text|
|Formatted inputs (e.g. email, IP address)| IP Address, URL, etc| Email, URL, IP Address|

### Sections 
For longer forms, it is helpful to organize the content into logical groups. For catalog item based forms, you can use the [Container](https://docs.servicenow.com/csh?topicname=r_VariableTypes.html&version=latest) capability to group sections. In a standard form, you can add sections in [Form Designer](https://docs.servicenow.com/csh?topicname=c_FormDesign.html&version=latest) or the [Form Layout](https://docs.servicenow.com/csh?topicname=configure-form-layout.html&version=latest)
 
### In-line Help 
Helping people easily complete a form ensures that the information entered is correct and completed efficiently. There are a few capabilities to consider helping users find success. 
 
#### For Forms
[Form annotations](https://docs.servicenow.com/csh?topicname=set-up-form-annotations.html&version=latest) are a way to provide inline instructions or information that a more advanced user can choose to hide. Annotations do not display in Service Portal. 

#### For Catalog Items
[Help text](https://docs.servicenow.com/csh?topicname=t_DefineAnItemQuestion.html&version=latest) provides additional information on a field when a user clicks on the “More information” link below the question.

### Data Validation and Error Handling
Good forms also handle data entry errors gracefully. When information doesn’t match the expected result, it is important to provide clear feedback to the user on how to resolve the situation. The best way to achieve this is through [Client Scripts](https://docs.servicenow.com/csh?topicname=client-scripts.html&version=latest) or [Catalog Client Scripts](https://docs.servicenow.com/csh?topicname=c_CatalogClientScriptCreation.html&version=latest) on the form that will require support from a developer. These scripts can display error or information messages based on JavaScript applied to filed values.

## References
Wroblewski, L. (2008). Web form design filling in the blanks. Rosenfeld Media.  
Jarrett, C. (2008, May 2). People before pixels: What to think about before you start. Effortmark. Retrieved June 16, 2022, from https://www.effortmark.co.uk/people-pixels/   


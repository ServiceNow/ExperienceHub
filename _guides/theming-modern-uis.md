---
title: Theming Modern UIs
share-description: With the Rome release, ServiceNow introduced UI Builder as the new platform to configure workspaces and portals based on the Next Experience framework. Many of ServiceNow’s own product leverage UI Builder to deliver their user experiences. In addition, if you are building a bespoke application using App Engine Studio, UI Builder will be the tool used to deliver Workspaces and Portals as part of your solution.
layout: page
permalink: /guides/theming-modern-uis
---

## Intro
With the Rome release, ServiceNow introduced [UI Builder](https://docs.servicenow.com/csh?topicname=ui-builder-overview.html&version=latest) as the new platform to configure workspaces and portals based on the [Next Experience](https://developer.servicenow.com/dev.do#!/reference/next-experience/ui-framework/getting-started/introduction) framework. Many of ServiceNow’s own product leverage UI Builder to deliver their user experiences. In addition, if you are building a bespoke application using [App Engine Studio](https://docs.servicenow.com/csh?topicname=aes-overview.html&version=latest), UI Builder will be the tool used to create or modify Workspaces and Portals as part of your solution.

If you are working with the AngularJS based Service Portal, please reference [Theming Service Portal Based UIs](/guides/theming-service-portals) for similar guidance.

If you want the applications you deliver to reflect your brand, you’ll want to understand how to apply the appropriate theme to the UIs delivered on ServiceNow. The UI Builder framework allows you to modify the colors, font, and logos used in the application. Partner with your own UI teams to understand how best to apply your theme to the UIs you deliver.

## Basic Setup
To begin, you need to ensure you are in the right scope for the application you want to modify. For example, in the guide below we’ll be modifying the Risk Portal that is part of the GRC Product Suite. You also need to have the right role assigned to your user (ui_builder_admin) to modify the theme setting.

1. To change application scope, log in to your ServiceNow instance and click the gear icon in the upper right of the window
2. Click on the Developer tab
3. In the Application dropdown, select the proper Application name. For this example, select GRC: Common Workspace Elements

*For more information about the application scope, see [Security and roles in UI Builder](https://docs.servicenow.com/csh?topicname=security-roles.html&version=latest).*

## How Themes Work
Each UI Builder based UI has a UX Theme Record associated with it. You can view all the themes on your instance by typing in sys_ux_theme.list into the Application Navigator. The theme record is a JSON object that consists of CSS variables as your object keys and the appropriate CSS values for the object value. Within a theme, you can override the core [Next Experience CSS variables](https://developer.servicenow.com/dev.do#!/reference/next-experience/rome/ui-framework/main-concepts/styles) 

**Note:** On this page the variables are shown with a “$” prefix, but in the theme record you will use “—” as well as create your own variables that you can use in a components Styles tab.

## Creating your first theme
 
1. In Application Navigator, search for “UI Builder” and open the UI Builder application
2. Click on Menu in the top bar
3. Select Edit Experience Settings
4. Go to Branding and theming
5. Click Create a Theme
6. Name your theme something memorable, you may want to apply this to other portals or workspaces later.
7. Enter a useful description to help your colleagues understand what this theme is for
8. In the “Theme” field is where you enter your CSS using the JSON format as described in [Create a Custom Theme](https://docs.servicenow.com/csh?topicname=create-theme.html&version=latest) and referencing the Next Experience CSS variables you want to modify.
9. Once you’re done modifying the theme record, click Update
10. Close and Reopen the Experience Settings pop up window.
11. Select Branding and Theming
12. Update the “Themes” dropdown to reference the new record you created.
13. Close the Experience Settings pop up window and click Open to see a preview of your changes

## Updating the Header
Once done modifying the JSON for the themes, you may want to replace the ServiceNow logo with your own. 

Stay in the Theme record and follow the instructions below.

1. Click on UX Theme Assets
2. Click on New
3. In the “Asset” field, click on the magnifying glass and in the pop-up, click on New. This will allow you to create a new Theme Asset
4. Set the Category to Image
5. Name your asset something memorable, you may want to use it in other themes.
6. Click the paperclip icon to attach the header image to the record
7. Click on Choose file to browse for your image file.
8. Once attached, close the Attachments pop up window
9. Click Submit
10. In the “Asset Properties” field, paste the follow JSON:

 `{ "position": "header_logo" }`

12. Return to the UI Builder tab and click Open to see a preview of your changes


## Changing the Font
Another common change you might want to make is updating your portal’s default font. This is done by adding a UX Theme Asset that holds the font file (of type: .ttf, .eof, .woff, etc) as an attachment and then updating your theme JSON to reference the new font. 

Stay in the Theme record and follow the instructions below.

1. Click on UX Theme Assets
2. Click on New
3. In the “Asset” field, click on the magnifying glass and in the pop-up, click on New. This will allow you to create a new Theme Asset
4. Set the Category to Image
5. Name your asset something memorable, you may want to use it in other themes. You’ll need to remember this asset’s name later in the process.
6. Click the paperclip icon to attach the font file to the record
7. Click on Choose file to browse for your image file.
8. Once attached, close the Attachments pop up window
9. Click Submit
10. Once the popup closes, click Submit again
11. You’ll return to the “UX Theme” page.
12. In the “Theme” field, add a new key-value pair with the key –now-font-family and the value the name you gave in step #5 above
13. Click Update
14. Return to the UI Builder tab and click Open to see a preview of your changes


At this point you’ve done some basic theming to make your portal better reflect your brand. To dive deeper into Theming, the following articles may be useful:

* [Change the brand and theme settings in your portal experience](https://docs.servicenow.com/csh?topicname=portal-branding-theme-settings.html&version=latest)
-	[Change the brand and theme settings in your workspace experience](https://docs.servicenow.com/csh?topicname=workspace-branding-theming-settings.html&version=latest)

# AI-Powered-Lead-Generation-System
The AI-Powered Lead Generation System is a Salesforce-based application that automatically identifies potential leads by analyzing customer data, website activity, and other business inputs. Using AI and Agentforce, it predicts which leads are most likely to convert, prioritizes them, and generates alerts or suggestions for sales reps.

Understanding Business Requirements

Description

Understanding Business Requirements involves identifying the goals, challenges, and expectations of the stakeholders to ensure the solution aligns with the organization’s objectives. This process includes gathering information through meetings, interviews, and research to define what the business needs to achieve and why. It focuses on clarifying key workflows, user roles, pain points, and desired outcomes. By translating business needs into clear, actionable requirements, this stage lays the foundation for designing a solution that delivers measurable value and supports strategic growth.
Defining Project Scope And Objectives

Defining Project Scope and Objectives involves outlining the boundaries, deliverables, and goals of the project to ensure clarity and alignment among all stakeholders. This stage specifies what will be included—and excluded—in the project, identifies key features, timelines, and resources, and sets measurable objectives. It ensures everyone understands the project’s purpose, expected outcomes, and success criteria. By establishing a well-defined scope and clear objectives, this phase helps prevent miscommunication, scope creep, and delays while guiding the project toward successful completion.


Salesforce Account
**Sign up for Dev Org**

Salesforce is your customer success platform, designed to help you sell, service, market, analyze, and connect with your customers. Salesforce has everything you need to run your business from anywhere. Using standard products and features, you can manage relationships with prospects and customers, collaborate and engage with employees and partners, and store your data securely in the cloud. So what does that really mean? Well, before Salesforce, your contacts, emails, follow-up tasks, and prospective deals might have been organized something like this: <https://youtu.be/r9EX3lGde5k> Creating Developer Account Creating a developer org in salesforce.

1. Go to <https://developer.salesforce.com/signup>

2. On the sign up form, enter the following details :

![image.png](https://skillwalletapp.s3.amazonaws.com/TCx3tYhHB/image.png)

1.First name & Last name 

[2.Email](http://2.Email) 

3.Role : Developer 

[4.Company](http://4.Company) : College Name 

5.County : India 

6.Postal Code : pin code 

Username : should be a combination of your name and company

This need not be an actual email id, you can give anything in the format : <username@organization.com> 

Click on sign me up after filling these. 

**Account Activation**

1. Go to the inbox of the email that you used while signing up. Click on the verify account to activate your account. The email may take 5-10mins.

![image.png](https://skillwalletapp.s3.amazonaws.com/YWB96vOYL/image.png)

2. Click on Verify Account

3. Give a password and answer a security question and click on change password.

![image.png](https://skillwalletapp.s3.amazonaws.com/8kuBXDXAI/image.png)


Objects Creation
1. Access Salesforce Setup

Log in to your Salesforce org.

Click the ⚙️ Gear Icon in the upper-right corner.

Select Setup from the dropdown menu.

You will be redirected to the Salesforce Setup Home.

2. Navigate to Object Manager

In the Setup menu, click Object Manager at the top navigation bar.

This will display a list of all standard and custom objects in the org.

3. Create a New Custom Object

Click Create → Custom Object (or click New Custom Object if visible).

The Custom Object Definition page will open.

4. Configure Custom Object Details

Fill in the following required fields:

Basic Information

Label: The display name of the object (e.g., Project).

Plural Label: (e.g., Projects).

Object Name: Auto-filled based on the Label.

Record Name:

Choose Text or Auto-Number.

If Auto-Number, define the format (e.g., PROJ-{0000}).

Optional Features (Enable Based on Use Case)

Allow Reports

Allow Activities

Track Field History

Allow Search

Allow Notes & Attachments

Enable Streaming API

Enable Enhanced Email

Deployment Status

Choose Deployed (available for use)

Or In Development (temporary, hidden from users)

5. Set Object-Level Security

Choose whether you want to:

Add Notes & Attachments

Allow Sharing

Enable Reports and Activities

Allow Bulk API Access

(These settings ensure users can interact with the object as intended.)

6. Save the Custom Object

Click Save.

The object is now created and you will be taken to its detail page.

Subtasks (1)
Milestone 2 : Objects and Fields

What is meant by object ?

In Salesforce, an object is essentially a database table that stores a specific type of information for an organization. It serves as a structured container for data, analogous to a spreadsheet where:

Objects: are like individual sheets or tables.

Fields: are the columns within those tables, defining the specific attributes or pieces of information to be stored (e.g., "Name," "Email," "Phone Number").

Records: are the rows within those tables, representing individual instances of the object (e.g., a specific "Account" record for "Acme Corp" or a "Contact" record for "John Doe").

Field Label

API Name

Data Type

Lead Score

Lead_Score__c

Number

Lead Category

Lead_Category__c

Picklist (Hot, Warm, Cold)

Product Interest

Product_Interest__c

Picklist(Training, Consulting, Certification)

AI Summary

AI_Summary__c

Long Text Area

Creation of Custom Fields

Step 3.1 :Click the Gear Icon → Setup

Step 3.2 : Click on the Object Manager

Step 3.3 : From the object list, Select Standard Object name is Lead

Step 3.4 : In the Lead object left menu, click Fields & Relationships and after click the New button.

Step 3.5 : Select the data type as Number → click Next.

Step 3.6 :Fill the Text details:

Field Label: Lead Score

Length:20

Click Next.

Step 6.7:Set Field-Level Security tick the Visible checkbox for profiles that should see the field (uncheck Read-Only if you want them to edit it).

Then click Next.

Step 6.8 : Click On The Save

Like this you need to create the remaining custom fields

Tabs:
Tabs in Salesforce are navigation elements that allow users to access specific objects, functionalities, or custom pages directly from the application interface.
They act as entry points that lead users to records, list views, Visualforce pages, Lightning components, or external content. Tabs help organize the workspace and make frequently used objects or tools easily accessible. Salesforce supports various types of tabs, including Custom Object Tabs, Web Tabs, Visualforce Tabs, and Lightning Page Tabs, each serving a different purpose in enhancing user navigation and experience.

1. Access Salesforce Setup

Log in to Salesforce.

Click the ⚙️ Gear Icon in the top-right corner.

Select Setup to open the Setup Home page.

2. Navigate to the Tabs Section

In the left-hand search bar, type Tabs.

Under User Interface, click on Tabs.

This page lists all available Standard Tabs, Custom Object Tabs, Visualforce Tabs, Lightning Page Tabs, and Web Tabs.

3. Create a New Custom Object Tab

Locate the section labeled Custom Object Tabs.

Click New.

The Custom Object Tab creation page will open.

4. Configure Tab Settings

Step A: Select the Custom Object

Choose the custom object you want to create a tab for (e.g., Project, Invoice, Application).

Step B: Choose a Tab Style

Select a Tab Style (icon + color) from the available options.

You can also create a custom tab icon if needed.

Step C: Enter Additional Information (Optional)

Add a description for internal reference.

Choose a custom splash page (rarely used).

5. Set Tab Visibility for Profiles

After selecting style and object, you will see tab visibility settings for each profile:

Choose one of:

Default On – visible in app navigation by default

Default Off – hidden but users can add it manually

Tab Hidden – completely hidden from profile

Set based on user access requirements.

6. Add the Tab to Custom Apps (Optional but Recommended)

After setting visibility, Salesforce will prompt you to assign the tab to Apps.

Select the apps where you want this tab to appear.

Click Save to complete the configuration.

7. Verify the Tab

After saving:

Go to the Salesforce App (e.g., Sales, Service, a custom Lightning App).

Click the App Launcher (9 dots icon).

Search for your custom object/tab.

Confirm that it displays correctly and users can create/view records.

Fields and Relationships :
Custom Fields Creation:

Field Label

API Name

Data Type

Lead Score

Lead_Score__c

Number

Lead Category

Lead_Category__c

Picklist (Hot, Warm, Cold)

Product Interest

Product_Interest__c

Picklist (Training, Consulting, Certification)

AI Summary

AI_Summary__c

Long Text Area

Steps: Creating the "AI Summary" Custom Field

Go to Setup

Log in to Salesforce.

Click the ⚙️ Gear Icon → Setup.

Open Object Manager

In Setup, click Object Manager (top navigation).

Search for and select the object you want to add the field to (Example: Lead, Custom Object, etc.).

Go to Fields & Relationships

In the left sidebar of the object, click Fields & Relationships.

Click the New button.

Choose Field Type

Select Long Text Area.

Click Next.

Enter Field Details

Fill in the field information:

Field Label: AI Summary

API Name: AI_Summary__c (auto-filled)

Length: Set max length (e.g., 32,768 characters)

Visible Lines: Choose the number of display lines (e.g., 5–10)

Click Next.

Set Field-Level Security

Select which profiles should have visibility or edit access.

Click Next.

Add to Page Layouts

Select the page layouts where the field should appear.

Click Save.

Like this you need to create the remaining custom fields

Creation of Custom Fields 

Step 3.1 :Click the Gear Icon → Setup

Step 3.2 : Click on the Object Manager

Step 3.3 : From the object list, Select Standard Object name is Lead

Step 3.4 : In the Lead object left menu, click Fields & Relationships and after click the New button.

Step 3.5 : Select the data type as Number → click Next.







Step 3.6 :Fill the Text details:

Field Label: Lead Score

Length:20

Click Next.

Step 6.7:Set Field-Level Security tick the Visible checkbox for profiles that should see the field (uncheck Read-Only if you want them to edit it). Then click Next.

Step 6.8 : Click On The Save

Like this you need to create the remaining custom fields

Application Creation :
A Salesforce application is a collection of tabs, objects, and tools grouped together to help users complete specific business processes. It provides a dedicated workspace where users can access all related data—such as accounts, contacts, opportunities, dashboards, or custom objects—without searching across the system. Applications can also be customized with logos, colors, and layouts to match an organization's branding while improving user experience and efficiency.

To create an application in Salesforce:
 Setup → App Manager → New Lightning App → Enter App Details → Choose Branding → Add Navigation Items → Add Utility Items (optional) → Assign to Profiles → Save & Finish.
 These steps guide you from opening the setup area to defining the app name, selecting tabs (objects), adding tools, choosing who can use the app, and finally making it available in the App Launcher for users.

Validation Rules :
Activity 1: To create a Validation rule to Lead Object

Click on Validation Rules → click on New.

Enter the Rule Name as Reject_Personal_Email.

Check Active.

Insert the Error Condition Formula as:

 OR(
  CONTAINS(Email, "@gmail."),
  CONTAINS(Email, "@yahoo."),
  CONTAINS(Email, "@hotmail."),
  CONTAINS(Email, "@outlook.")
)
Enter the Error Message as:
 “Personal email domains like Gmail, Yahoo, Hotmail, and Outlook are not allowed.”

Select the Error Location as Email.

Click Save.

Flows
Steps to Create the Record-Triggered Flow

From Setup, in the Quick Find box, search for Flows.

Click New Flow.

Select Category: Triggered.

Select Type: Record-Triggered Flow.

Configure the Start Element:

Object: Lead

Trigger: A record is created or updated

Entry Condition Requirements: (example based on common lead email use cases—adjust to match your flow)

Optimize the Flow For:
 Actions and Related Records

When to Run the Flow:
 Run Immediately

6. Click Done.

7. Add the Email Action

Add the Send Email Action

6.1 Click the + icon below the Start element.

6.2 Select Action.

6.3 In the Action search bar, type:

Send Email

6.4 Select: Send Email

6.5 Configure the action fields:

Label: Send Lead Email

Subject: (enter your email subject)

Body: {{!$Record.Name}}

{!$Record.AI_Summary__c}

Recipient Addresses: (enter email formula or field reference; e.g., {!$Record.Email})

Sender Type: Org-Wide Email or Default

Is HTML Body: True

RecordId → {!$Record.Id} (if included in your setup)

Click Done and Activate.

Agentforce

Create Prompt Template

Click the Gear Icon → Select Setup.

In the Quick Find box, search Einstein Setup.

Click Einstein Setup.

Enable Turn on Einstein.

Refresh the page after enabling Einstein.

Prerequisite: Create AI_Summary__c Field

Before selecting the field in Prompt Builder, you must create the AI Summary Custom field in the Lead Standard Object.

Steps:

Click Gear Icon → Setup.

In Quick Find, search Object Manager.

Select Lead

Click Fields & Relationships → New.

Select Long Text Area → Click Next.

Field Label: AI Summary

API Name auto-populates as AI_Summary_c

Set Length = 32000 and Visible Lines = 5–10.

Click Next → Save.

Step 2: Open Prompt Builder

In the Quick Find box, search Prompt Builder.

Click Prompt Builder.

Click New Prompt Template.

Step 3: Select Prompt Type

Choose Field Generation.

Label Name:AI Summary Field Generation Field

API Name auto-populates.

Object:Lead

Field: AI Summary.

Step 5: Insert Resources

Full Name: {!Lead.Name}

Company: {!Lead.Company}

Email: {!Lead.Email}

Phone: {!Lead.Phone}

Lead Source: {!Lead.LeadSource}

Lead Status: {!Lead.Status}

Description: {!Lead.Description}

Step 6: Enter Sample Prompt

Write the below prompt:

Generate a detailed summary of this Lead using the selected fields.

Explain the Lead’s background, company information, contact details, status, source, and any key notes clearly.  

Summarize relevant details such as the current engagement stage, potential interest level, communication history, and any important remarks.

Provide the summary in a clean, structured, and easy-to-understand format.

Step 7: Save and Activate

Click Save.

Click Activate.

Your Prompt Template is now ready.

Activity 2 : Deploy Prompt Builder in Visa Application Object Using Lightning App Builder.

Step 1: Open Any Record

Click the App Launcher (9 dots).

Search for Lead Object

Open any existing Student Record.

Step 2: Edit Lightning Page

Click the Gear Icon → Select Edit Page.

Step 3: Upgrade to Dynamic Detail Page

Click the Detail Page.

Click Upgrade Now.

Click Next.

Select the Lead Object Layout.

Click Finish.

Step 4: Assign the Prompt Template to the Field

Click the AI_Summary_c field on the layout.

In the right-side panel, search Prompt Template.

Select your template: AI Summary Field Generation Field

Step 5: Save & Activate the Page

Click Save.

Click Activate.

Select Assign as Org Default.

Choose Desktop and Phone.

Click Next.

Click Save.

Click Back.

Activity 3 : Testing to Lead object Record

For the AI Summary field, click the icon in the last corner. That is the AI icon we created using Prompt Builder.

2 .Click Stars Icon on AI Summary Field

3. Click Use

4. Click Save.

UI/UX Development and Customization :

UI/UX Development & Customization focuses on designing and building intuitive, visually appealing, and user-friendly interfaces that enhance the overall user experience. This stage includes creating wireframes, prototypes, and layouts, followed by customizing design elements such as colors, typography, components, and interactions to match brand identity. It ensures smooth navigation, accessibility, responsiveness across devices, and seamless integration with backend functionality. The goal is to create an engaging, efficient, and consistent user journey that aligns with both user needs and business objectives.
Profiles:
. Access Salesforce Setup

Log in to Salesforce.

Click the ⚙️ Gear Icon in the top-right corner.

Select Setup to open the Setup Home.

2. Navigate to Profiles

In the left-hand Quick Find search box, type Profiles.

Under Users, click Profiles.

A list of all available profiles (Standard and Custom) will be displayed.

3. Select the Profile to Modify

From the profile list, click the Profile Name you want to configure
(e.g., System Administrator, Standard User, Custom Sales Profile).

This opens the Profile Detail page.

4. Configure Profile Permissions

On the Profile Detail page, you can configure:

A. Object Permissions

Click Object Settings

Select the object (e.g., Lead, Custom Object)

Set Read, Create, Edit, Delete, View All, Modify All

B. Field-Level Security

Click Field Permissions or go to an object → View Field-Level Security

Control field visibility and edit access

C. Tab Settings

Scroll to Tab Settings

Set each tab to Default On, Default Off, or Tab Hidden

D. App & System Permissions

Scroll to Administrative Permissions

Scroll to General User Permissions

E. Record Type Assignments

Click Record Type Settings (if available)

Assign or remove record types

5. Save Profile Changes

After completing the required updates, scroll down.

Click Save to apply the changes.

6. (Optional) Clone Profile to Create a Custom Profile

From the Profiles list, click Clone next to an existing profile.

Give the new profile a name.

Configure permissions as needed.

Save.

A profile is a group/collection of settings and permissions that define what a user can do in salesforce. Profile controls “Object permissions, Field permissions, User permissions, Tab settings, App settings, Apex class access, Visualforce page access, Page layouts, Record Types, Login hours & Login IP ranges. You can define profiles by the user's job function. For example, System Administrator, Developer, Sales Representative.

Activity 1: Create Lead Manager Profile
Go to Setup → type Profiles in Quick Find → click Profiles.

Click Clone next to Standard User.

Enter:

Profile Name: Lead Manager Profile

Click Save.

Edit the profile:

Under Object Settings, enable Read, Create, Edit, Delete access for:

Lead

Task

Event

Contact

Enable Modify All on Lead (optional based on requirement)

Ensure API Enabled is checked

Click Save.

Activity 2: Create Sales Agent Profile
Go to Setup → Profiles


Click Clone next to Standard User


Enter:


Profile Name: Sales Agent Profile


Click Save


Edit permissions:


For Lead → allow Read, Create, Edit


Remove Delete permissions


Allow access to: Task, Event


Ensure View Reports is enabled


Click Save

Users
Users — Navigation Steps

1. Access Salesforce Setup

Log in to Salesforce.

Click the ⚙️ Gear Icon in the top-right corner.

Select Setup to open the Setup Home page.

2. Navigate to Users

In the left-hand Quick Find search box, type Users.

Under the Users section, click Users.

A list of all active, inactive, and frozen users will be displayed.

3. Create a New User

At the top of the Users list, click New User.

Fill in the required information:

First Name

Last Name

Alias

Email

Username

Nickname

Role (optional)

User License

Profile

Scroll down and click Save.

4. Edit an Existing User

In the Users list, click Edit next to the user you want to update.

Make the necessary changes
(profile, role, email, active status, time zone, etc.).

Click Save.

5. Activate, Deactivate, or Freeze a User

A. Deactivate a User

Click Edit beside the user.

Uncheck Active.

Click Save.

B. Freeze a User (Temporary Lock)

Click the Freeze button next to the user’s name.
(This prevents login without deactivating the user.)

6. Reset a User Password

On the Users list, click the Reset Password button beside the user.

Salesforce sends the user a password reset link via email.

7. Assign Permission Sets (Optional)

Open the user record by clicking the User Name.

Scroll to Permission Set Assignments.

Click Edit Assignments.

Add or remove permission sets.

Click Save.

Roles  :
 Access Salesforce Setup

Log in to Salesforce.

Click the ⚙️ Gear Icon in the top-right corner.

Select Setup to open the Setup Home.

2. Navigate to Roles

In the Quick Find search bar (left panel), type Roles.

Under Users, click Roles.

The Role Hierarchy page will open, showing existing roles in a tree structure.

3. Create a New Role

On the Role Hierarchy page, click Add Role.

Choose a parent role (if applicable) to determine visibility and hierarchy.

Enter role details:

Role Name

Role Label

This role reports to: (set parent role)

Optional: Add a Description

Click Save.

4. Edit an Existing Role

On the Role Hierarchy page, find the role you want to modify.

Click the Edit link beside the role name.

Update the role name, parent hierarchy, or description.

Click Save.

5. Assign Users to a Role

In the Role Hierarchy, click the role name.

On the role details page, scroll to the Users in This Role section.

Click Add.

Select one or more users from the list.

Click Save.

Data Migration, Testing & Security  :
Data Migration, Testing & Security ensures the system is reliable, accurate, and protected before going live. This phase involves securely transferring existing data into the new system, validating its integrity, and resolving inconsistencies. Comprehensive testing—functional, performance, usability, and integration—verifies that all features work as intended and meet requirements. Security measures such as encryption, access control, vulnerability checks, and compliance validation are implemented to protect data and prevent unauthorized access. The goal is to deliver a stable, high-quality, and secure solution ready for deployment.

User Adoption and Change Management  :

User Adoption and Change Management focuses on preparing users for new systems, processes, or tools and ensuring they embrace and effectively use them. It involves planning clear communication, providing role-based training, and offering continuous support to help users understand the benefits of the change. Through stakeholder engagement, pilot testing, feedback collection, and ongoing reinforcement, this process reduces resistance, improves user confidence, and ensures a smooth transition from old workflows to new ones. Effective change management increases system usage, enhances productivity, and maximizes the overall value and return on investment of the implemented solution.

Project Documentation :

Project documentation serves as the comprehensive written record of all key details, activities, decisions, and deliverables throughout the project lifecycle. It includes requirement specifications, design documents, development steps, testing reports, deployment guidelines, user manuals, and maintenance procedures. Its purpose is to ensure clarity, consistency, and transparency among stakeholders while providing a reliable reference for future enhancements or troubleshooting. Well-structured documentation streamlines communication, supports smooth knowledge transfer, and helps maintain the long-term sustainability and scalability of the system.


Guidelines For Project Documentation and Submission  :

Guidelines for Project Documentation and Submission ensure that all project materials are organized, accurate, and presented in a professional manner. Documentation should follow a consistent structure, include clear headings, and provide complete details such as requirements, architecture, configuration steps, testing results, and deployment instructions. All screenshots must be properly labeled, and any code or configurations should be formatted and explained. The final submission should be compiled into a clean, logically arranged document or folder, with all files named appropriately and delivered by the specified deadline. Following these guidelines ensures quality, readability, and easy evaluation of the project.

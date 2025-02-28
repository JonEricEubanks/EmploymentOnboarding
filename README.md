# NEO Employment Onboarding App

## Overview
The **NEO Employment Onboarding App** is a streamlined, automated solution designed to manage the onboarding process for new employees within local government organizations. Built using **Microsoft Power Platform**, this application ensures a **structured, efficient, and transparent onboarding experience** for HR, IT, managers, and new employees.

## Features
- **Automated Onboarding Workflow**: Tracks all onboarding tasks across HR, IT, and department managers.
- **Task Assignment & Tracking**: Provides clear task lists with progress tracking.
- **Notifications & Alerts**: Uses Power Automate to send email reminders and status updates.
- **Integration with Microsoft 365**: Works seamlessly with SharePoint, Outlook, and Teams.
- **Data Insights & Reporting**: Includes Power BI dashboards to monitor onboarding trends.
- **Role-Based Access Control**: Ensures security by restricting access based on roles.

## Technology Stack
The application is built using the **Microsoft Power Platform**, utilizing:
- **Power Apps**: Provides the front-end interface for onboarding task management.
- **Power Automate**: Automates notifications, approvals, and workflow processes.
- **SharePoint**: Serves as the backend for storing onboarding-related data.
- **Power BI**: Enables visualization of onboarding progress and analytics.

## Installation & Deployment
### **Prerequisites**
- Microsoft Power Platform environment with Power Apps, Power Automate, and Power BI.
- SharePoint Online for data storage.
- Admin access to configure necessary permissions.

### **Deployment Steps**
1. **Import the Solution**
   - Download and unzip the **EmploymentOnboardingApp.zip** file.
   - Navigate to **Power Apps** > **Solutions** > **Import Solution**.
   - Select the `.zip` file and follow the import wizard.

2. **Configure SharePoint Lists**
   - Create required SharePoint lists for **New Hires**, **Task Assignments**, **HR Approvals**, etc.
   - Update the Power Apps data sources to connect to your SharePoint site.

3. **Set Up Power Automate Flows**
   - Navigate to **Power Automate**.
   - Ensure all onboarding automation flows are activated and connected to the correct SharePoint lists.

4. **Assign Security Roles**
   - Configure role-based permissions for HR, IT, Managers, and New Employees.

5. **Test the Application**
   - Run test onboarding cases to ensure the workflows and approvals function correctly.

## Usage Guide
1. **HR Creates a New Hire Record**
   - HR enters new employee details, start date, and assigns an onboarding workflow.

2. **Tasks Assigned to IT, Managers, and HR**
   - Automated tasks are assigned based on predefined workflows.

3. **New Employee Completes Self-Registration**
   - New hires log in to complete required forms and training modules.

4. **Progress Tracking & Completion**
   - Managers can track onboarding status, and HR can ensure all steps are completed.

## Troubleshooting
- **Missing Data Connection?** Ensure SharePoint list names match what is referenced in Power Apps.
- **Emails Not Sending?** Verify Power Automate flows are correctly enabled.
- **Permissions Issue?** Check user roles and access levels in Power Apps settings.

## Future Enhancements
- Integration with **Microsoft Teams Chatbot** for onboarding assistance.
- AI-driven **Copilot recommendations** for improving onboarding efficiency.
- Expanded analytics with **Power BI predictive insights**.

## 
NEO Employment Onboarding App - Setup Instructions

Prerequisites

Microsoft Power Platform environment with Power Apps, Power Automate, and Power BI.

SharePoint Online for data storage.

Admin access to configure necessary permissions.

Setup Instructions

Step 1: Import the Solution

Download the EmploymentOnboardingApp.zip file.

Navigate to Power Apps > Solutions > Import Solution.

Select the .zip file and follow the import wizard.

Step 2: Create a SharePoint Site

Navigate to SharePoint Admin Center.

Click Create Site and select Team Site.

Name the site "Employment Onboarding" and configure necessary access permissions.

Step 3: Configure SharePoint Lists and Libraries

Create the following Document Library:

App Training Videos

Title (Single line of text)

Description (Multiple lines of text)

UniqueId (Single line of text) - This must be updated for training videos.

Reference video: https://www.youtube.com/watch?v=-IHzq0vJHWU&t=528s

Create the following Lists with Required Columns:

Administrators

Name (Single line of text)

Email (Single line of text)

Role (Choice: HR, IT, Manager, Employee)

Permissions Level (Choice: Read, Edit, Full Control)

Departments

Department Name (Single line of text)

Manager (Person/Group)

Department Code (Single line of text)

Location (Single line of text)

New Employee List

Employee Name (Single line of text)

Job Title (Single line of text)

Department (Lookup: Departments List)

Start Date (Date/Time)

Manager (Person/Group)

Onboarding Status (Choice: Not Started, In Progress, Completed)

Task Assignments

Task Name (Single line of text)

Assigned To (Person/Group)

Due Date (Date/Time)

Status (Choice: Not Started, In Progress, Completed)

Related Employee (Lookup: New Employee List)

Task Category

Category Name (Single line of text)

Description (Multiple lines of text)

Active (Yes/No)

Tasks

Task Name (Single line of text)

Category (Lookup: Task Category)

Description (Multiple lines of text)

Required for Role (Choice: HR, IT, Manager, Employee)

URLs

Title (Single line of text)

URL Link (Hyperlink)

Description (Multiple lines of text)

Category (Choice: Internal, External, Training, Resources)

Ensure Power Apps is configured to connect to these lists and libraries.

Step 4: Set Up Power Automate Flows

Navigate to Power Automate.

Ensure all onboarding automation flows are activated and connected to the correct SharePoint lists.

Step 5: Assign Security Roles

Configure role-based permissions for HR, IT, Managers, and New Employees.

Step 6: Test the Application

Run test onboarding cases to ensure the workflows and approvals function correctly.

Contact & Support

For further support, contact the IT Helpdesk or your Microsoft 365 administrator.




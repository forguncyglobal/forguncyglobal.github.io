---
layout: default
title: Workflows
parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/Workflows/
nav_order: 8
---

# {{ page.title }}

Here, you can streamline the application approval process by configuring the business processes flow. Various activities in an organization require approval from superiors and heads. The workflow console allows you to create an application approval process based on organizational structure and user information specified in User Service. 

Forguncy provides easy-to-use workflow functionalities where you can create different states and define rules for each state. The workflow functionalities are offered to the user by a [Process Bar](https://docs.forguncy.net/develop/Cell-types/Process-bar/) cell type. 


- [Overview](#overview)
- [Set Up The Workflow](#set-up-the-workflow)
- [New Normal (Simple) Process](#new-normal-simple-process)
- [New Approval (Complex) Process](#new-approval-complex-process)

## Overview

The flow of a series of business processes is called **Workflow**. Workflows are different processes that automatically share documents, information, or tasks between multiple participants under some predefined rules to achieve a particular business goal.

Let's consider a scenario where an employee submits a business trip application. After submitting the application, it will be shared with the managers or heads for approval. Later, the details will be sent to the accounts department. 

With Forguncy you can create such states and define rules for the approval process. Try [Business Trip](http://localhost:4000/getting-started/sample-(templates)/#business-trip) sample to understand the workflow console of Furguncy.

Note: Workflows require user management to configure rules. So you need to use Forms Authentication or Windows Domain Authentication and add users to User Management. 
{: .note}
![workflow-settings](/assets/images/product-images/workflow-settings.png)

## Set Up The Workflow
### Procedure
1. Open a data table and go to **Table Settings**. Click on **Workflows..** to open **Workflow Settings** dialog box.
2. Check **Enable** in the Workflow Settings dialog to use the workflow function.
3. Under **Status** tab, set all the status that may appear in the workflow. *New*, *Waiting Approval*, and *Approved* are the default status. Use **+** or **-** to add or delete status, and up and down arrows to change the order of the status. 

    Note: The first state is used for the initial state of the record, and the other states can be customized in their order. The number of states can also be changed, but must include both the initial state and the end state. 
    {: .note}
4. Set workflow process under **Process** tab. There are two types of process: **New Normal (Simple) Process** and **New Approval (Complex) Process**. Both can be used for the approval process and allows creating a rule that takes a record from one state to another state based on an action that is executed in certain condition. But the **New Approval (Complex) Process** allows you to create more complex rules such as: 
    - Configure rule per approver (by specifying name)
    - Define further workflow such as what automated actions to perform on Approval and Rejection respectively.
    - Can perform automated actions before and after the transfer from one approver to another.
5. Click on **OK** to save the workflow settings. 
6. User Setting is necessary in the workflow process. Register the user (who are involved in the workflow) in the **User Service** before doing the workflow settings.

    Note: You can register roles and extended attributes for each user. Select users, roles, and extended attributes to specify what they can handle.
    {: .note}

![workflow-settings](/assets/images/product-images/workflow-settings-duedates-reminders.png)

#### [Back To Top](#workflows)

## New Normal (Simple) Process 

To add a Normal (Simple) process, select a process row and click on Add Normal (Simple) Process tab. A new row will be added after the selected process row. 
Set rule and conditions for the process through below settings described in Table: 
Processes can be added or deleted with **+**, **-** within columns. 

![workflow-settings](/assets/images/product-images/workflow-settings-new-normal-process.png)

#### Table: Normal Process Settings 

|Setting|Description|
|:--|:--|
|From state|The state of the workflow before the action is executed.|
|Action |Set the actions that the person in charge can perform. The set action is displayed as a button that can be executed by the person in charge in the workflow bar set on the page. You can set multiple actions for one selected process by selecting the process in the list and clicking [+] in the action column. However, be careful not to duplicate the action name in one process.|
|In Condition |It is used to change the "state after execution" or the next "person in charge" depending on the conditions. When you add a condition, the characters set for the action will be displayed as buttons in the workflow bar. For example, if the amount is 50,000 yen or more, the person in charge is the boss (action is set to "submit boss"), if it is less than 50,000 yen, the person in charge is accounting (action is set to "submit accounting"), and so on. Allows you to change the person in charge of the next process. In the workflow bar, two buttons of "submit boss" and "submit accounting" set for the action are displayed.|
|Command|You can set commands before and after executing an action. The commands that can be set are page transition, email transmission, table data update, conditional branching, JavaScript code execution, message display, and repeat command. However, you cannot specify page cells with commands that use formulas.|
|Approval type|Set whether only one person can approve or all the people need to approve.|
|To state|Defines the state of the workflow after the action is performed.|
|Assign To| Defines the person responsible for the next process after the action is taken. <br/> Display the drop-down list and choose from the list on the Roles> Custom> Users tab. <br/> If you have set a user account type field in the table, it will be displayed custom. <br/> If you select a role name in the "Role" tab of the above screen, the "Filter based on organizational information" checkbox will be displayed at the bottom of the screen. Check here to filter the people responsible for the next process by organization by logged-in user. If you don't want to filter by logged-in user, you can click Advanced ... to select other filter criteria such as author, last modifier, or user column in the table. <br/> In the red frame above, you can set the workflow bar to allow you to make the following selections: <br/> -[Select one from the above users] You can select one of the users set in "Person in charge" as the next person in charge. <br/> -[All the above users] All the users set in "Person in charge" will be the next person in charge. <br/> When any one of them executes the process, it will transition to the next state. <br/> * Not all configured users need to perform the following processing.| 


#### [Back To Top](#workflows)

## New Approval (Complex) Process

If you need to approve multiple roles, you can make your workflow easier by using the Approval Process instead of adding multiple steps to the Normal Process. Also, if the workflow includes you as an approver and you are applying as an applicant then in the case of the Normal process, you need to approve yourself even if you are the applicant which logically is not the correct process. However, in the Approval process, you can skip your approval step and proceed to the next . 

To add a Approval (Complex) process, select a process row and click on Add Approval (Complex) Process tab. A new row will be added after the selected process row. 
Set rule and conditions for the process. For the **From state**, **Conditions**, **To state**, **Assign To** settings , refer to the normal process settings.
Processes can be added or deleted with **+**, **-** within columns. 
Click the "Approval Process ..." hyperlink to set the details as mentioned in below table:

![workflow-settings](/assets/images/product-images/workflow-settings-new-approval-process.png)
![workflow-settings](/assets/images/product-images/workflow-settings-approval-process-settings.png)
#### Table: Approval Process Settings 

|Setting|Description|
|:--|:--|
|Applicant |Specifies who will start the approval process. You can choose from the author or user account type fields.|
|Add/Delete/Move up/Down approvals|You can add/remove approval stages. Click the up and down arrows to change the order of approval stages.|
|Approver |The person who will approve the request. <br/>Select the role of the approver. Role settings are in **User Services**, see [Users & Roles](http://localhost:4000/user-services/Users-&-roles/#users--roles).|
|Based on organization Filter |Whether approvers are filtered based on the organization nodes in which the applicant is located. For more information about the structure and level of your organization, see Create an organization structure.|
|Approval enter condition |The requirements for the records submitted by the applicant to enter this approval process.|
|Approval Command Settings |Set up commands before or after approval process transfers, before or after rejecting process transfers.|
|Multi Approval Policy |If there are multiple approvers in the approval process, you can select <br/> **Choose One Approval**: Select one of the approvers in the approver list to approve the record.<br/> **Any One Approval**: Any person in the approver list can approve the record. After that the stage ends and proceeds to the next step. Similar to  the **Choose one of the user above** in the Normal processes.<br/> **All Approval**: The entire list of approvers approves the record before the stage ends and proceeds to the next step. Similar to the **All of the users above** effect in the Normal process.|
|RejectPolicy |If the approval is rejected, it can be reset to<br/>**BacktoStart**: Returns the request directly to the start state.<br/> **BacktoPreStep**: Takes back to previous step.<br/> **Finishprocess**: Closes the application directly and end the process.|
|For Approval/Rejection|Customizes the approve/ reject button text.| 






 



 

 

 





 



 

 




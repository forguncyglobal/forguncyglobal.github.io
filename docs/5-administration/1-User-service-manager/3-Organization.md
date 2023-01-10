---
layout: default
title: Organization
parent: User Service Manager
grand_parent: Administration
permalink: /administration/User-service-manager/uorganization/
nav_order: 3
---

# {{ page.title }}

After defining users and their roles, the next task is to create an organization and its department or groups. 

In user service manager, the organizational structure is divided into two sections- **Levels** and **Organizations**. You can build hierarchical structure of an orgainzation under **levels** option. It allows you to create different levels for branches, divisions, and teams. The **Organizations** option creates group unit of an organization such as sales department, development group, testing team, accounts, and more. 

![levels and organization](/assets/images/product-images/levels-organization.png)
{:.dropshadow}

## How to create organization Levels

### Adding levels

Steps to **Add** organization levels are as follows:

- On the User Service Manager screen, go to **Levels**.
- Click **Add levels**

![organization-add-levels](/assets/images/product-images/organization-add-levels.png)
{:.dropshadow}

- Enter *Level Name* in the dialog box and click *OK* to save. You can see that the Organization level has been added to the list.
- The *Cancle* button allows you to cancle the process. 

![organization-add-levels-dialog](/assets/images/product-images/organization-add-levels-dialog.png)
{:.dropshadow}

You are allowed to create as many levels as you required. 

### Editing and Deleting levels

Steps to **Edit** or **Delete** an organization level name are as follows:

- On the User Service Manager screen, go to **Levels**.
- Place the mouse cursor over the organization level name you want to edit or delete. 
- Choose the right icon and proceed. 

![organization-edit-delete-levels](/assets/images/product-images/organization-edit-delete-levels.png)
{:.dropshadow}


## Organization

You can register in a hierarchical structure based on the structure of the organization from "Organization" in the user account management screen menu, and assign an " organization level " to each organization. Then, by assigning each user belonging to that organization

When you select the "Organization" menu on the user account management screen, the following screen is displayed.

![organizations](/assets/images/product-images/organizations.png)
{:.dropshadow}

1. Assign an organization name and organize the organization into hierarchies. See Adding Organizations.
2. Specify a user who belongs to the organization selected in (1).

Note: Since, automatic save processing is performed on every 5 seconds, in most cases changes will not be discarded even if the **Save** button is not clicked.
{:.note}

### Adding Organization

Steps to **Add** an organization are as follows:

- On the User Service Manager screen, go to **Organization**.
- By default, *organization 1* is displayed in the initial state.
- Click the icons to the right of the organization name for the **Edit**, **Delete**, or **Add** operations.

    **Edit** option allows you to edit the organization name. <br/>
    **Delete** option deletes the  organization.<br/>
    **Add** allows you to add levels and create hierarchy in the organization

- Assign levels to your organization by clicking the name for which you want to set the organization level, and select value from the **Level** combo box on the right.

Note: The enteries saved in [Level](#adding-levels) are reflected under **Level** combo box. 
{:.note}

- [Add members](#adding-members) belonging to the organization.
- By clicking on the level name, you can see the users belong to.

![organization-levels-users](/assets/images/product-images/organization-levels-users.png)
{:.dropshadow}

### Adding Members

Steps to add members in an organization are as follows:

- Select the organization you want to add members to.
- Click the **Add Members** button.
- Select an authentication method and add a users.
- Check the check box you want to designate user as the *Supervisor* of the organization. Supervisors have lower privileges than users in parent organization nodes and higher privileges than users in child organization nodes.
- Sets the member's organizational role from the **Organization Role** drop-down list.
- Click the **Save** button to commit your changes.

![organization-add-members](/assets/images/product-images/organization-add-members.png)
{:.dropshadow}

### Remove Member

Steps to delete an added member in an organization are as follows:

- Hover on the member you want to delete from the list.
- Click **Delete**. 

![organization-add-members](/assets/images/product-images/organization-add-members.png)
{:.dropshadow}


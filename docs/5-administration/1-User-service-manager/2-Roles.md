---
layout: default
title: Roles
parent: User Service Manager
grand_parent: Administration
permalink: /administration/User-service-manager/role/
nav_order: 2
---

# {{ page.title }}

**Role** means a group with common responsibilities and privileges such as *Administrator*, *System Owner*, and *Temporary Staff*. It is used to manage permissions for each group to determine what operations can be performed on the application. You can specify groups privileges by assigning them a role.

![roles-add](/assets/images/product-images/roles-add.png)
{:.dropshadow}

Note: The Administrator is a default role that is registered in the system. You cannot delete this role.
{:.note}

## Adding Role

Steps to **Add** roles are as follows:

- On the User Service Manager screen, go to **Roles**.
- Click **Add Role**.
- Enter role name and save it with **OK** button. Click **Cancle** to cancle the process.

You can see the added role in the list below **Add Role** button. 

![role-add-dialog](/assets/images/product-images/role-add-dialog.png)
{:.dropshadow}

## Editing and Deleting Role

Steps to **Edit** or **Delete** an organization level name are as follows:

- On the User Service Manager screen, go to **Roles**.
- Place the mouse cursor over the organization level name you want to edit or delete. 
- Choose the right icon and proceed. 

![role-edit-delete](/assets/images/product-images/role-edit-delete.png)
{:.dropshadow}

## Adding Members

Steps to specify roles to members are as follows:

- On the User Service Manager screen, go to **Roles**.
- Select the target role from the list of roles, and click the **Add Members** button.

Note: A user belonging to the *Administrator* role has the same privileges as an *Administrator* user.
{:.note}

- Select an authentication method and add a users. From the combo box, select whether to add a *Forms authentication* or *Windows authentication* user.

![role-add-members](/assets/images/product-images/role-add-members.png)
{:.dropshadow}

Note: You can add both *Forms Authentication* and *Windows Authentication* users to a single role. However, you can only add users with either authentication method in a single addition operation. 
{:.note}

## Removing a Member

Steps to remove a member assigned to a role are as follows:

- Select the target role and hover on the member you want to delete from the list.
- Click **Delete**. 

![role-delete](/assets/images/product-images/role-delete.png)
{:.dropshadow}

Note: *Administrators* can not be removed from a role. 
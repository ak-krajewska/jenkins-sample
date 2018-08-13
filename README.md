Jenkins - Create and Manage Users
=================================

This section of will teach you how to create new users and to manage their permissions using the Role Strategy Plugin. 

Table of Contents
-----------------
* [Create Users](#create-users)
* [Download and Install the Role Strategy Plugin](#download-and-install-the-role-strategy-plugin)
* [Enable Role-Based Strategy](#enable-role-based-strategy)
* [Create Roles](#create-roles)
* [Assign Roles to Users](#assign-roles-to-users)

Create Users
------------

1. Log into Jenkins as an administrator. 
2. In the main Jenkins menu on the left, select **Manage Jenkins**. 
3. Select **Manage Users**. You will see a table of current users.
4. In the main menu on the left, select **Create User**.
5. Fill in the form with the new user's name, password, full name, and email address. Click **Create User** below the form.
6. You will return to the table of users. If you wish you can click the cogwheel icon next to any user to configure the account, including changing the name and password.

*In most situations, you will want granular user permissions. If you don't need granular user permissions, you can stop here.* 

Download and Install the Role Strategy Plugin
---------------------------------------------

*If you have already downloaded and installed the Role Strategy Plugin, proceed to Enable Role-Based Strategy.*

1. In the main Jenkins menu on the left, select **Manage Jenkins**.
2. Select **Manage Plugins** from the list of options.
3. Select the **Available** tab, and type “Role Strategy” in the search box. 
4. Select the checkbox next to **Role Strategy** and click **Download now and install after restart**.
5. Once the confirmation screen displays the message “Downloaded Successfully,” select the checkbox next to **Restart Jenkins**. 
6. Log in again as an administrator. 

Enable Role-Based Strategy
--------------------------

1. In the main Jenkins menu on the left, select **Manage Jenkins**.
2. Select **Configure Global Security** from the list of options.
3. Select the checkbox next to **Enable security**.
4. In the Authorization section, select the radio button next to **Role Based Strategy**. (If that option isn't available, verify that you have downloaded and installed the Role Strategy Plugin.)
5. Click **Apply** and then **Save**. You will return to the Manage Jenkins menu. 

Create Roles
------------

1. In the main Jenkins menu on the left, select **Manage Jenkins**.
2. Select **Manage and Assign Roles** from the list of options.
3. Select **Manage Roles**.
4. Decide if you would like to create a Global Role or a Project Role. Global Roles provide authorization and access on a global level to your entire Jenkins instance while Project Roles provide authorization and access to specific projects within it. 
5. Enter a name for your new role. If it's a Global Role, click **Add**. If it's a Project Role, enter the regular expression pattern for the projects that the role will be allowed to access, and then click **Add**. 
6. Select checkboxes corresponding the level of permissions you'd like for your new role.
7. Click **Save**.

Assign Roles to Users
---------------------

1. Navigate to the **Manage and Assign Roles** menu again: Main Menu => Manage Jenkins => Manage and Assign Roles.
2. Select **Assign Roles**.
3. Enter the name of the user you wish to add to a group, either in the Global roles section for a Global Role, or the Item roles section for a Project Role. Click **Add**.
4. In the **User/group** table, select the role you wish to assign to the new user.
5. Click **Apply**, and then **Save**.

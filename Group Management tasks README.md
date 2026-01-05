# Group Management tasks
As you continue your journey at Contoso, your next task involves managing groups to efficiently organize users and streamline access to resources. In this lab, you create a security group and a Microsoft 365 group. These groups ensure that users are properly categorized based on their roles and responsibilities. You add users to these groups and assign licenses to ensure they have access to the necessary resources. Group management tasks are essential for maintaining a structured and secure environment within Microsoft Entra. This allows you to manage permissions and resources more effectively.

## Task 1 - Create a Microsoft 365 group
1. Open the Microsoft Entra admin center at https://entra.microsoft.com.
2. Log in using the credentials for your tenant.
3. From the menu on the left, select `Groups` and then `All groups`.
4. Select `New group` option.
5. Enter the requested information:
```
Field	                                   Value
Group type	                             Microsoft 365
Group name	                             Project23
Group description	                       This group consists of members of the new AI Simulation software with codename Project23
Membership type	                         Assigned
```
6. Under the `Members` heading, select `No member selected`.
7. Add `Bhogeswar Kalita`, by marking the box and choosing the `Select` button.
8. Select the `Create` button.
<img width="500" height="840" alt="image" src="https://github.com/user-attachments/assets/488d173a-fc84-469a-b0b0-99d015ec1502" />
<img width="500" height="358" alt="image" src="https://github.com/user-attachments/assets/2a4a1b2a-38c2-4e23-a25b-8a38f12c423f" />

---
## Task 2 - Create a Security group
1. Open the Microsoft Entra admin center at https://entra.microsoft.com.
2. Log in using the credentials for your tenant.
3. From the menu on the left, select `Groups` and then `All groups`.
4. Select `New group` option.
5. Enter the requested information:
```
Field	                                Value
Group type	                          Security
Group name	                          Guest Users
Group description	                    This group has all the Guest users currently in the tenant.
Membership                            type	Dynamic User
```
6. Under the `Dynamic user members` heading, select `Add dynamic query`.
7. Create a dynamic query with the following values:
```
Field	                                Value
Property	                            userType
Operator	                            Equals
Value	                                Guest
```
8. Select the `Save` item from the top of the page.
9. Select the `Create` button.
`Note` - It will take up to 2 minutes for the group to be populate.

10. From the `Groups` select the `Refresh` item.
11. Select the `Guest Users` group we just created.
12. Select `Members`.

---
## Task 3 - Add an existing user to a new group
1. Open the Microsoft Entra admin center at https://entra.microsoft.com.
2. Log in using the credentials for your tenant.
3. From the menu on the left, select `Groups` and then `All groups`.
4. Select the `Project23` group we created in Task 1.
5. Select the `Members` option from the menu.
6. Select `+ Add members` from the menu near the top.
7. Mark the box next to `External User` and use the `Select` button.
<img width="500" height="796" alt="image" src="https://github.com/user-attachments/assets/88eec4f0-63ad-4452-b1b3-a119dd3ed6e8" />

## Subtask 1 - Alternative method to add an existing user to a new group
1. Open the `Users` menu, then select `All users`.
2. Find and select `External User` from the list.
3. Select the `Groups` item from the menu.
4. Select the option to `+ Add memberships`.
5. Mark an existing group and use the `Select` button to add them.
<img width="500" height="412" alt="image" src="https://github.com/user-attachments/assets/e98e497f-3e01-4406-ae15-3fabfed74891" />

----
## Task 4 - Add licenses and owners to a group
1. Open the Microsoft Entra admin center at https://entra.microsoft.com.
2. Log in using the credentials for your tenant.
3. From the menu on the left, select `Groups` and then `All groups`.
4. Select the `Project23` group we created in Task 1.
5. Choose the `Owners` option from the menu.
Note - Your tenant administrator will automatically be added as the owner of a group, if no owner is specified.

6. Select the `+ Add owners` menu item.
7. Mark the box next to `Bhogeswar` and use the `Select` button.
8. Notice the new owner has been added to the group.

## Subtask 1 - Adding a license to a group
1. Open a new tab in your browser.
2. Connect to Microsoft 365 admin cetner at https://admin.microsoft.com.
3. From the menu on the left, open the `Billing` section and select `Licenses`.
4. Select the `Microsoft Power Automate Free` license.
5. Choose the `Groups` tab from the newly opened screen.
6. Select the `+ Assign licenses` item.
7. Use the dropdown on the right side of the screen to select the `Project23` group created earlier.
8. Use the `Assign` button at the bottom of the screen.
9. Close the `You assigned licenses…` notification.
10. Use the `Refresh` button to see the added group licenses.
<img width="500" height="804" alt="image" src="https://github.com/user-attachments/assets/9ccbd2fb-6c3c-445f-9770-3dedb9ee7677" />



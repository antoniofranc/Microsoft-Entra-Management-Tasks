# Perform basic User Management tasks

In your new role at Contoso, you're tasked with managing user accounts. You ensure that employees and external partners have the necessary access to company resources. Your first assignment involves creating a new user account, adding a license to enable access to essential services. Next, you're inviting an external user to collaborate on a project. After that, you assign a specific role to a user to grant appropriate permissions. Finally, you perform a bulk import of users and user data to streamline the onboarding process. These tasks are fundamental to maintaining an organized and secure identity management system within Microsoft Entra.

## Task 1 - Create a new user
1. Open the Microsoft Entra admin center at https://entra.microsoft.com.
2. Log in using the credentials for your tenant.
3. From the menu on the left, select  `User` and then  `All users C.
4. Select +  `New user ` and then pick the  `Create new user` option.
5. Enter the requested information:
```
Field                                                  Value
User principal name                                    Bhogeswark
Display name                                           Bhogeswar Kalita
```
6. Leave the `Mail nickname` as is.
7. Make a copy of the Password (auto-generated) and store it in Notepad. You will need it later.
8. Leave Accounted enabled checked.
9. Select the Properties tab.

<img width="500" height="849" alt="image" src="https://github.com/user-attachments/assets/22338f52-b033-4ff7-af70-13243b53e5c2" />

10. Set the values for first and last name:
```
Field                                                  Value
First name                                             Bhogeswar
Last name                                              Kalita
```
11. Note that you can set the `User type` to `Member`. If you pick Guest, it will restrict the users capabilities.
12. Scroll down to the bottom of the page.
13. Set the `Usage location` to `United States` or to whatever region you are in.
14. Select the `Review + create` button.
15. Select `Create`.

<img width="500" height="505" alt="image" src="https://github.com/user-attachments/assets/d83cc416-b460-4069-870b-867ee82ec81c" />


## Subtask 1 - Log in to confirm user
1. Open an InPrivate browsing window.
2. Connect to the Microsoft Entra admin center at the link https://entra.microsoft.com.
3. Enter the username and password you just created.
```
Field                                                  Value
Username                                               Bhogeswark@ your tenant name .onmicrosoft.com
Password                                               Auto generated passsword you saved
```
4. If prompted follow the on-screen instructions to complete MFA setup.
5. Feel free to explore the Microsoft Entra admin center for a minute.
6. Close the InPrivate browsing window.
------
## Task 2 - Add a license to the user
1. Open a new tab in your browser.
2. Connect to the Microsoft 365 admin center at https//:admin.microsoft.com.
3. If prompted, log in using the credentials for your tenant.
4. Find the menu on the left side of the screen.
5. Open the `Billing` item in the menu.
6. Select `Licenses` from the list.
7. When the list of licenses appears, select `Microsoft Power Automate Free`.
8. Select the `+ Assign licenses` item.
9. Choose `Brogeswar` from the list (user created in previous task).
10. Select the `Assign` button at the bottom of the page.
11. Notice the message that you have successfully assigned a license.
12. Close the tab with `Microsoft 365 admin center`.
<img width="500" height="483" alt="image" src="https://github.com/user-attachments/assets/f2d364cc-e93a-459a-9c25-d2ed833e3f5f" />

-----
## Task 3 - Invite an external user to your tenant
1. If not already open - Open a browser and connect to the Microsoft Entra admin center at https://entra.microsoft.com.
2. If prompted, log in using the credentials for your tenant.
3. From the menu on the left, open the `Identity` menu.
4. Select `Users` then select `All users`.
5. At the top of the page select `+ New User`.
6. Choose the option to `Invite external user` from the dropdown.
7. Enter the information for your new external user:
```
Field                                                  Value
Email                                                  ExUser@testemail.com
Display name                                           Exeternal User
Message	                                               Thank you for joining the company for this short work project. We look forward to building this project together.
```
8. Select the `Review + Create` button.
9. Select `Create`.
<img width="500" height="847" alt="image" src="https://github.com/user-attachments/assets/8bd49958-4dde-4164-8d46-cc3327f93954" />

----
## Task 4 - Assign a role to a user
1. If not already open - Open a browser and connect to the Microsoft Entra admin center at https://entra.microsoft.com.
2. If prompted, log in using the credentials for your tenant.
3. In the left menu find the `Identity`  section. Open it if not already opened.
4. Select `Users`  then select `All users` .
5. Choose the user `Bhogeswar Kalita`  create in the earlier task.
6. From the newly opened menu select `Assigned roles` .
7. At the top of the screen select `+ Add assignment`.
8. From the `Select role`  dropdown menu chose the role `Attribute Definition Reader` .
9. Select the `Next`  button when it becomes available.
10. Choose the option `Eligible`  for `Assignment type` .
11. Select `Assign` .
<img width="500" height="846" alt="image" src="https://github.com/user-attachments/assets/121af966-e76b-4645-9801-4c20a9d07afa" />

## Subtask 1 - Alternate method to assign a role to a user
1. Look at the Identity menu section on the left side of the screen.
2. Select the `Show more` option to see the full `Identity` menu.
3. From the list of items in the `Identity` menu, expand the `Roles & admins` section.
4. Select `Roles & admins`.
5. Select `Attribute Log Reader` from the list of roles.
6. From the top of the screen select `+ Add assignment`.
7. From the `Select member(s)` select the `No member selected` text.
8. From the list of user choose `Bhogeswar Kalita`.
9. Choose the `Select` button at the bottom.
10. Select the `Next` button.
11. On the Add assignments page choose `Active` for the `Assignment type`.
12. Note that you have to enter a justification for this role / user assignment.
13. Enter the justification `User will be working as an Attribute log reader as their primary job`. into the box.
14. Select `Assign`.
<img width="500" height="852" alt="image" src="https://github.com/user-attachments/assets/53d0f151-4e08-484d-91f3-7fbf0c1c3913" />

-----
## Task 5 - Bulk import users
1. If not already open - Open a browser and connect to the Microsoft Entra admin center at https://entra.microsoft.com.
2. If prompted, log in using the credentials for your tenant.
3. From the `Identity` menu, select `Users` and then select `All users`.
4.From the top of the page, select the `Bulk operations` drop-down arrow and then select `Bulk create`.
`Note` - Selecting Bulk create will open a new tile. This tile provides a Download link to a template file that you will edit to populate with your user information and upload to add the bulk creation of users.

5. Select `Download` to see a sample bulk user CSV file.
`Note` - The .csv template provides you with the fields included with the user profile. This includes the required username, display name, and initial password. You can also complete optional fields, such as Department and Usage location, at this time. You do not need to fill out all the fields.
`Lab Tip` - A sample CSV has been provided in the Allfiles/Lab1 folder – APL0501-BulkUser.csv.

6. Open Notepad.
7. Open the SC300BulkUser.csv file.
8. Search and replace the existing value **«>>** with **Your actual domain name**.
9. Save the file.
10. On the Bulk create users dialog, select the file folder icon on step 3.
11. Path to the Allfiles/Lab1 folder and select `APL0501-BulkUser.csv` file.
12. Select `Open`.
13. Wait for the notification that the file uploaded successfully. Select the `Submit` button to add the users.

Note - After the users have been created, you will be prompted that the creation has succeeded.

14. `Close` the `Bulk create users` dialog.
15. Check the list of users to see your bulk created users.
<img width="500" height="597" alt="image" src="https://github.com/user-attachments/assets/594659c5-996e-4a6a-87e0-d135751be036" />

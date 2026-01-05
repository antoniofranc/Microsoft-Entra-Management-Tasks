# Multifactor Authentication tasks
As you advance in your role at Contoso, you're now responsible for managing Multifactor Authentication (MFA) settings to enhance the security of user accounts. In this lab, you enable and disable per-user MFA settings. Enabling MFA ensures users have an extra layer of protection when accessing company resources. You review MFA settings such as Trusted IPs to allow secure access from specific locations. Finally, you configure MFA lockout settings to prevent unauthorized access attempts and protect sensitive information. These tasks are crucial for maintaining a secure and resilient identity management system within Microsoft Entra.

## Task 1 - Enable / Disable Per-user MFA settings
1. Open the Microsoft Entra admin center at https://entra.microsoft.com.
2. Log in using the credentials for your tenant.
3. From the menu on the left, open the `Identity` submenu
4. Select `Users` and then select `All users`.
5. Look at the menu on the top of the new screen and find `Per-user MFA`.
6. Select `Per-user MFA`.
7. Put a mark in the box next to `Bhogeswar Kalita`.
8. Select `Enable MFA` from the top of the list.
9. Read the message box that pops up.
`Note` - This is a manual URL that you can email to the user, if you want to let them know to set up MFA.

10. Select `Enable` button.
11. Note that after a few seconds `enforced` shows up next to Bhogeswar’s name.
<img width="500" height="758" alt="image" src="https://github.com/user-attachments/assets/95797e3e-e9c8-431b-a373-4c076f0f61ab" />

----
## Task 2 - Review the Service settings for MFA
1. Open the Microsoft Entra admin center at https://entra.microsoft.com.
2. Log in using the credentials for your tenant.
3. From the menu on the left, open the `Identity` submenu.
4. Select `Users` and then select `All users`.
5. Select `Per-user MFA` item.
6. Select `Service settings`.
7. Review the settings you can configure
```
Setting	                                               What is it for
App passwords	                                         There are some legacy apps that won’t work with MFA, use this setting to allow a user to keep using them.
Trusted IPs                                            If your company has a specifc set of IP-address ranges that are always known safe, you can allow users to by-pass MFA the logging in.
Verification options	                                 Select the methods you are willing to allow users to use for their second factor of authentication.
Remember multifactor authentication on trusted device	 If your users are using a device that you trust, like a company managed laptop; you can allow them to retain thier MFA approved status for a specified number of days.
```
8. Select the `Discard` button if you made any changes.
9. This is one method of configuring MFA for your users.
<img width="500" height="756" alt="image" src="https://github.com/user-attachments/assets/3c85f0e8-5249-4bd5-ac7b-97b5cd9200f9" />

-----
# Task 3 - View MFA account lockout settings
1. Open the Microsoft Entra admin center at https://entra.microsoft.com.
2. Log in using the credentials for your tenant.
3. From the menu on the left, open the `Protection` submenu.
4. Scroll to the bottom of the list and select `Show more`.
5. Select `Multifactor authentication` from the menu.
6. Select `Account lockout` from the menu.
7. Set the following lockout values:
```
Field	                                              Value
Number of MFA denials to trigger account lockout	  3
Minutes until account lockout counter is reset	    180
Minutes until account is automatically unblocked	  15
```
8. Select the Save option at the top of your screen.
9. Review some of the other configuration options you have on MFA like:
- Fraud alert
- Block / unblock users
- Notifications

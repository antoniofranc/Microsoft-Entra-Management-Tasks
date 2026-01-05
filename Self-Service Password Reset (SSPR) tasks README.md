# Self-Service Password Reset (SSPR) tasks

As you continue to enhance the security measures at Contoso, your next task is to configure and enable Self-Service Password Reset (SSPR). This feature allows users to reset their passwords independently, reducing the workload on the IT support team. This change improves overall security and efficiency. In this lab, you enable SSPR, configure the necessary settings, and ensure that only the designated users have access. By implementing SSPR, you empower users to manage their passwords securely and conveniently.

## Task 1 - View the SSPR properties for a specific group
1. Open the Microsoft Entra admin center at https://entra.microsoft.com.
2. Log in using the credentials for your tenant.
3. From the menu on the left, open `Protection` submenu and then select `Password reset`.
4. Find the `Self service password enabled` bar.
```
Value	What it means
None	No users can use the SSPR feature
Selected	Only members of the selected group(s) can use SSPR
All	All users can use the SSPR feature
```
5. Set the value to `Selected`.
6. Select the text `No groups selected`.
7. Mark the `Project23` group we created previously.
8. Use the `Select` button to complete your choice.
9. `Save` your configuration.

## Subtask 1 - View SSPR authentication methods
1. Select `Authentication methods` from the menu within `Password reset`.
2. Select `1` as the value for `Number of methods required to reset`.
`Note` - this value represents how many different ways the user is required to sign-in to the password reset tool, before they are allowed to reset their password. Note that using a password is not an option.

3. Select `Email, Mobile phone, and Mobile app code for Methods available to user`.
Note - if you use Security Questions you have to specific the number of questions the user is required to create and answer.

4. Use the button at the top to `Save` your choices.
5. You have added an Authentication method to your self-service password reset.

## Subtask 2 - View SSPR registration
1. Select `Registration` from the menu within `Password reset`.
2. Make sure the `Require users to register when signing in?` value is set to `Yes`.
3. Set the `Number of days before users are asked to re-confirm…` to `90` days.
4. Select `Save` to save your changes.

## Subtask 3 - View SSPR reset notifications
1. Select `Notifications` from the menu withing `Password reset`.
2. Leave the `Notify users on password reset?` at the default of `Yes`.
3. Change the `Notify all admins when other admins reset their password?` value to Yes.
4. Use the `Save` option to save your changes.

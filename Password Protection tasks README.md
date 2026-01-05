# Password Protection tasks

As you progress in your role at Contoso, you're now responsible for enhancing the security of user accounts by implementing password protection measures. In this lab, you enable the password protection feature in Microsoft Entra. You need to set lockout values to prevent unauthorized access attempts. Next you review custom banned passwords to ensure that users create strong and secure passwords. These steps are crucial for safeguarding sensitive information and maintaining the integrity of the company's systems.

## Task 1 - View lock settings, and review duration and threshold values
1. Open the Microsoft Entra admin center at https://entra.microsoft.com.
2. Log in using the credentials for your tenant.
3. From the menu on the left, select `Protection` submenu and then select `Authentication methods`.
`Note` - You could also search on `Password protection` in the search bar at the top.

4. Select `Password protection` from the list.
5. Set the `Custom smart lockout` with the following values.
```
Field	             Value	    Description
Lockout threshold	 5	        How many times can you fail to login with a password before your account locks.
Lockout duration	 30	        How many second the account should lock when the threshold is reached.
```
`Note` - You can also configure a custom banned password list here.

6. Set `Enforce custom list to `Yes`.
7. Enter the following values:
- Contoso
- London
- Widget
`Lab Tip` - Your lab is being performed for a company called Contoso, located in London, and it makes Widgets. By enter these three words you block them from being part or a whole of a password.

8. Set the value for `Mode` to `Enforced`.
9. Select the `Save` item at the top of the screen.
<img width="500" height="748" alt="image" src="https://github.com/user-attachments/assets/dcea068f-9550-4d7c-8160-13d85085ffcc" />

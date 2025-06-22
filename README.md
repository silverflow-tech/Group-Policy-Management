# Group-Policy-Management

For this project, I will be creating new GPOs regarding password complexity, account lockout, and restricting users to Control Panel

Prerequsites: 

Windows 2022 Installation > https://github.com/silverflow-tech/Windows-2022-Installation

Active Directory Configuration > https://github.com/silverflow-tech/Active-Directory-Configuration

Step 1: Go to the search bar at the bottom and type 'Group Policy Management' and open the application

![image](https://github.com/user-attachments/assets/bfda79f9-2df6-4888-82aa-75a5bdb5d50f)

Step 2: Click on your forest > Domains > name.local > right click on your domain > Create a GPO in this domain...

![image](https://github.com/user-attachments/assets/4791e305-7205-477d-a66e-019a8d403563)

Step 3: I'm going to start with 'Password Complexity'. You can name it whatever you like, but make sure you it's straightforward so you don't get confused in the future

![image](https://github.com/user-attachments/assets/2295d051-a82b-4edc-8d83-4fea75995dd8)

Step 4: After creating the new GPO, right click on it and select 'Edit'

![image](https://github.com/user-attachments/assets/a49a7936-a5e0-4ea9-890d-af49f6c73f04)

Step 5: Go to Computer Configuration > Polices > Windows Settings > Security Settings > Account Policies. You should see the screenshot below 

![image](https://github.com/user-attachments/assets/368253ca-77cc-406d-9505-0f820a952a9e)

Step 6: Select 'Password Policy' and you'll see the screenshot below. You can determine what the conditions are going to be. 

![image](https://github.com/user-attachments/assets/bb99d563-ed29-450c-a661-19caed55a06f)

Step 7: Right click on a category and determine the conditions/values you want to enter. Apply and click 'OK'. These are the conditions I've made for my GPO

![image](https://github.com/user-attachments/assets/2ce2e6a2-1696-4fcf-8e28-89eb6cb195ee)

Step 8: Now that the password complexity has been configured, I'm going to set the conditions for account lockout. Go back to the previous page and click on 'Account Lockout Policy' 

![image](https://github.com/user-attachments/assets/5f73f288-ed69-4614-8b84-ac2177b86d9d)

Step 9: These are the configurations I've applied. To change each one, right click on the cateory and select 'Properties'. Enter the value > Apply > Ok.

![image](https://github.com/user-attachments/assets/2defe3eb-1c38-4a17-8d70-e7730c7f1e96)

The Password Complexity GPO is now complete and I'm going to create another policy to restrict users access to Control Panel

Step 10: Go back to your domain and select 'Create a GPO in this domain...'

![image](https://github.com/user-attachments/assets/c7af8909-6814-4cc1-9699-55e899c85959)

Step 11: Name your new GPO, mine is going to be 'Restrict Control Panel'. Make sure it's clear and concise

![image](https://github.com/user-attachments/assets/ebf83bd6-32ef-4787-9183-10870e4471cc)

Step 12: Right click on your new policy and select 'Edit'. Go to User Configuration > Administrative Temp > Control Panel 

![image](https://github.com/user-attachments/assets/64d356fa-8747-4089-bc4f-9d1f477c253e)

Right click on 'Prohibit access to Control Panel and PC settings' and select 'Edit'. Select 'Enabled' and see the change after you exit. 

![image](https://github.com/user-attachments/assets/561dc299-81b2-4b3a-a789-8978cb2da2f4)

This completes the project. 



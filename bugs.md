
##bug01
Description:Incorrect header for Phone number Verification

Page/Functionality: Login/Sign-up page 6-digit Code Verification screen

page url: https://linqapp.com/welcome

User: New User/Existing User

Severity: Low

Steps to Reproduce:
1. Navgiate the GUID
2. Enter the Valid Phone Number
3. Click on Continue
4. Look for the header value on the page

Expected: User should see "Confirm Phone Number" as the header on the page while validating the 6-digitcode received to their phpne..
Results: User is seeing "Confirm Email" as the header on the page while validating the 6-digit code received to their Phone.






##bug02

Description: Required feild items on Sign-Up page are missing mandatory(*)sign

Page/Functionality: Name and Email Address fields on sign-up page

page url: https://linqapp.com/welcome

User: New User

Severity: Low

Steps to Reproduce:
1. Naviagte the URL
2. Enter the Valid phone number
3. Click on continue
4. Enter the 6-digit code and verify the number
5. click on continue
6. Fill out the required fields and hit on continue

Expected: User should be able to identify the required fields, First and Last Name and Email Address fields with mandatory(*) sign. 
Results: User is not able to see the required fields with mandatory(*) sign and if try to continue without filling the Name and email address, it is giving required field error. 







##bug03

Description: Add contact info is not throwing error while adding same contact in profile preview

Page/Functionality: Edit contact page "Add Contact Information" 

Url: https://linqapp.com/welcome

User: New/Existing User

Severity: Major

Steps to Repo:
1. Navigate through the url
2. Enter the Phone Number
3. Hit on Continue
4. Validate the number and continue
5. Enter the Name and Email on sign up page and continue if New User
6. Skip the line 5 if Existing User and continue
7. Click on "Edit Contact" on the profile landing page
8. Scroll down and click on Add Contact Info
9. Select any option and enter the details
10. Save the information added
11. Hit on "Save Changes" to the profile
12. Repeate line 8-11 with same contact information

Expected: User should not able able to add the same contact information. If the phone/email/address/link/custom field data matches with the new contact information data, User should be notified with an error message "data already exists".
Results: User is not throwing any sort of error messages and is able to add multiple contact info's with same data.








##bug04

Description: Required feild items on Add Contact Information are missing mandatory(*)sign

Page/Functionality: Phone Number, Email, Address, Link and Custom information fields inside Add Contact Info

page url: https://linqapp.com/welcome

User: New User/ Existing User

Severity: Low

Steps to Reproduce:
1. Naviagte the URL
2. Enter the Valid phone number
3. Click on continue
4. Enter the 6-digit code and verify the number
5. click on continue
6. Fill out the required fields and hit on continue
7. Skip the line 5 if Existing User and continue
7. Click on "Edit Contact" on the profile landing page
8. Scroll down and click on Add Contact Info
9. Select any option
10. On the Information modal add data to the required fields 
11. Hit on Save

Expected: User should be able to identify the required (*) fields to be filled before hitting the save button on the information page. 
Results: User is not seeing any required field(*) on the information page but when try to save without adding the data user is receiving the error message "uh oh! a filed value is required"






##bug05

Description: Dropdown Action button missing to change country on welcome page

Page/Functionality: Phone number entered on the welcome page is auto considering as United States Number

Url:page url: https://linqapp.com/welcome

User: New User/ Existing User

Severity: Critical

Steps to Reproduce:
1. Naviagte the URL
2. Enter the Valid phone number which is NOT unitedstates(+1)
3. Click on continue

Expected: User should be able to enter any valid phone number NOT ONLY United States. User should be able select there preferred country while entering the number by clicking on the country icon.

Results: Any valid number out of United states is ingesting the number with +1, considering as United States Number. User is not able to select their preferred country.








##bug06

Description: Login/Sign-up is rendered as plain text instead of clickable URLs

Page/Description: Welcome page login/sign-up is are missing click event

url: https://linqapp.com/welcome

User: NEW/Existing User

Severity: Major

Steps to Repo:
1. Navigate throught the url
2. Click on Login if Existing User
3. Click on Sign-up if New User

Expected: User should be redirected to login/sign-up page according to their preferred click.
Results: User is not able to redirect to login/sign-up page due to missing action handlers.





##bug 07
Description: Missing Guest User flow

Page/Description: Welcome page is missing Guest User flow

url: https://linqapp.com/welcome

User: NEW User

Severity: Medium

Steps to Repo:
1. Navigate throught the url
2. Observe the landing page as an new user
3. Notice only Login and Sign-up options are present
4. There is no "Continue as Guest" option available

Expected: User should be able to explore limited features without beign forced to login or signup.
Results: User is only able to Login or Sign-up. No option available for Guest access.




# Onboarding-automation
Overview - Onboarding System setup via Power Automate

1. Manager's Approval workflow
At first we have created an automated flow for the Manager's approval.
The approval mail is sent as soon as an onboarding form is filled by the HR or management body .
In order to achieve this I have created an excel sheet and I have inserted the 'Onboarding form'within the Excelsheet. Sample image is given below
![image](https://user-images.githubusercontent.com/116060032/220829740-d19cbba9-9af0-4892-98a6-3d853bb3bdcc.png)
As you can see the log for all the newly added user is maintained on this excel sheet. The time is recorded 

The sample of the onboarding form is here as shown below -

![image](https://user-images.githubusercontent.com/116060032/220858032-e90b5208-9072-4ff7-9c16-26907b3e1c7e.png)


As soon as the form is submitted with the required fields then an automated mail will be sent to the Assigned Manager . Here the important point to note here is that the manager who has been assigned in the onboarding form ;the flow will take that action as dynamic. Therefore the mail will be sent to that person only.
Image of approval workflow via Power Automate - 
![image](https://user-images.githubusercontent.com/116060032/220855943-6999863c-27d0-47ee-b473-329d02674cb3.png)

After someone submits the form  a mail is sent for approval where two buttons will be there. The assigned Manager has to pick any one of the given two options.
 Below is the image of mal that will be received by the Assigned Manager.
![image](https://user-images.githubusercontent.com/116060032/220831381-9de8919d-35d8-40bf-9bab-62816adc44c0.png)
As you can see the mail is received . 

2.Send the Onboarding Update to the User's personal Email ID - Next action is to either approve or Disapprove the onboarding. 
Case 1- If he approves then the congratulations mail is sent to the newly onboarded user's personal email id where the details regarding get started document and a formal form .These two will be included within the body of the mail. This form will further be used to add another flow to create the user to the project specific Channel.
Case 2- If the manager diapproves onboarding then also the info will be shared with the user.
Here is the image of the mail received after Manager approves onboarding.

![image](https://user-images.githubusercontent.com/116060032/220836991-4211555f-cff6-40f7-acd8-384cdc4ed446.png)

3. To create work items on azure board for the new joinee via Power automate - AS you can see above there is an another form attached within the body of the mail.This form will be used as an input to trigger another action.The form will be  redirected to create azure work items.That means as soon as the person submits the form before that the task must be defined for him in the azure_work_item_flow so that after he submits he gets notified via mail regarding details of the tasks.
The flow image is shown below-
![image](https://user-images.githubusercontent.com/116060032/220838819-04ea29ff-23d0-4da2-ace5-0fa175f10ad6.png)
Here the task will be created for the user as soon as he submits the form received on his mail.
![image](https://user-images.githubusercontent.com/116060032/220858677-9b753526-496a-440a-9d07-fb6c6076738a.png)

The image of created azure work items via Power Automate is shown below
![image](https://user-images.githubusercontent.com/116060032/220856777-aee4380f-a40d-414f-a01f-c1758d7992df.png)


4. Add the newly onboarded person to the project specific channel - At the end the user gets added to a separate channel created on microsoft Teams.
As sson as the person gets added a welcome message is automatically sent within the channel to introduce with the Entire Team.






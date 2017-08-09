# Reading Starred Results in Salesforce
Starred does not support Integration to read Starred feedback response into Salesforce yet. However, we using Starred Webhooks with Zapier you can create a Zap which will allow you to make this integration possible.

Please follow this guideline to build integration between starred and Salesforce to read Starred data in Salesforce.

## Requirements
1. Starred account. (sign up [here](https://app.starred.com/en/registration/register) if you don't have an account)
2. Salesforce account. (For testing purposes using [Salesforce developer account](https://developer.salesforce.com/signup?d=70130000000td6N) is highly recommended)
3. [Zapier Account](https://zapier.com/sign-up).

## Step by Step Guide

### Section 1. Setup a Webhook trigger in Zapier
1. In Zapier Dashboard click on 'Make a Zap' in Topbar. This brings you to Zapier Editor
2. In left Sidebar, you can see some options.
3. Give a name to this Zap in 'Name your Zap...' input field.
4. Next, we have to setup a Trigger.
5. Choose App: Webhooks
6. Choose Trigger: Catch Hook (Wait for a new POST, PUT....)
7. Click Save + Continue
8. Leave Setup Options blank unless you want to grab a child key from data Object.
9. On Test this Step interface you will see a URL.

![alt text](https://github.com/starred-com/salesforce/blob/salesforce-zap/Reading%20Starred%20Results%20in%20Salesforce/Section-1-Step-9.png "Section 1 Step 9")

### Section 2. Setup Callback URL in Starred

1. Go to Account Settings in Starred Platform (app.starred.com).
2. From Sidebar on the left click "API".
3. Scroll Down to Webhooks Section.
4. Paste the URL from Step 9 in Section 1 in Callback URL field.
5. Select 'Post form data' radio button.
6. Click Save.

![alt text](https://github.com/starred-com/salesforce/blob/salesforce-zap/Reading%20Starred%20Results%20in%20Salesforce/Section-2-Step-4.png "Section 2 Step 4")


**Optional Steps to Get test data in Zapier.**
* Head to Forms and send an invite to yourself.
* Fill in Survey form that you received in your email.

### Section 3. Test your Webhook in Zapier
_We will pick up where we left off in step 9. in Section 1_

1. On 'Test this Step' interface click 'OK, I did this'.
2. Zapier will listen to Webhook and will get collect data when triggered.

### Section 4. Setup Salesforce Action in Zapier
1. In 'Choose an Action App' select Salesforce.
2. In Select, Salesforce Action Select the Action you want to create.
3. In 'Select Salesforce Account' Interface Connect your Salesforce account. (We recommend connecting developer account for testing purposes)
4. Configure The template for the Salesforce Action and click 'Continue'.
5. In Test This Step you can click 'Create & Continue' to Test this Integration or click 'Skip Test & Continue'.

_Congratulations, you have successfully Integrated Starred feedback data with Salesforce._

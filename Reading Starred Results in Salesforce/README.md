# Reading Starred Results in Salesforce
Starred does not support Integration to read Starred feedback response into Salesforce yet. However, we using Starred Webhooks with Zapier you can create a Zap which will allow you to make this integration possible.

Please follow this guideline to build integration between starred and Salesforce to read Starred data in Salesforce.

##Requirements
1. Starred account. (sign up [here](https://app.starred.com/en/registration/register) if you don't have an account)
2. Salesforce account. (For testing purposes using [Salesforce developer account](https://developer.salesforce.com/signup?d=70130000000td6N) is highly recommended)
3. [Zapier Account](https://zapier.com/sign-up).

##Step by Step Guide

###Section 1. Setup a Webhook trigger in Zapier
1.1. In Zapier Dashboard click on 'Make a Zap' in Topbar. This brings you to Zapier Editor
1.2. In left Sidebar, you can see some options.
1.3. Give a name to this Zap in 'Name your Zap...' input field.
1.4. Next, we have to setup a Trigger.
1.5. Choose App: Webhooks
1.6. Choose Trigger: Catch Hook (Wait for a new POST, PUT....)
1.7. Click Save + Continue
1.8. Leave Setup Options blank unless you want to grab a child key from data Object.
1.9. On Test this Step interface you will see a URL.


###Section 2. Setup Callback URL in Starred

2.1. Go to Account Settings in Starred Platform (app.starred.com).
2.2. From Sidebar on the left click "API".
2.3. Scroll Down to Webhooks Section.
2.4. Paste the URL from Step 1.9 in Callback URL field.
2.5. Select 'Post form data' radio button.
2.6. Click Save.


** Optional Steps to Get test data in Zapier.**
* Head to Forms and send an invite to yourself.
* Fill in Survey form that you received in your email. 

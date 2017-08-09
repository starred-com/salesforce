# Salesforce Default Templates
The following files can be used to get started with integrating Starred with Salesforce.

## About Salesforce
Salesforce uses APEX triggers for updating objects, these triggers are also required for sending out feedback from Starred via Salesforce.
To get started, it's necessary to set up a APEX Class and an APEX trigger in your Salesforce Sandbox. The code required for this can be found in this repository.
Furthermore you're required to specify which tags/properties you're willing to send to Starred. For example:
- Email, FirstName, LastName contact are default
- Contact Owner (Full Name)
- Accountnaam
- Subject ticket
- Case manager
- Status = closed

## Reading Starred Results in Salesforce
Sending Starred results back in to Salesforce is currently not supported, but can be achieved very easily through Zapier.
To achieve this, you will need a working Zapier account, and use their [Webhook Zap](https://zapier.com/zapbook/webhook/) in combination with [Starred Webhooks](https://app.starred.com/api). Currently, this only works when you've opted to post Form data, instead of JSON data.

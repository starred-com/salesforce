# Sending out feedback from Starred via Salesforce
Salesforce uses APEX triggers for updating objects, these triggers are also required for sending out feedback from Starred via Salesforce.

## About Salesforce
To get started, it's necessary to set up a APEX Class and an APEX trigger in your Salesforce Sandbox.

The code required for this can be found in this repository.

Furthermore you're required to specify which tags/properties you're willing to send to Starred. For example:
- Email, FirstName, LastName contact are default
- Contact Owner (Full Name)
- Accountnaam
- Subject ticket
- Case manager
- Status = closed

## Reading Starred Results in Salesforce
Sending Starred results back in to Salesforce is currently not supported, but can be achieved very easily through Zapier.
Please follow the [Reading Starred Results in Salesforce]() guide.

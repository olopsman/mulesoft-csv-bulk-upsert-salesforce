# Mule Bulk Update Job from CSV

## Check CSV sample in the project for reference
## Have a valid salesforce account
## Create a creds.properties file in the src/resources/ directory
`Fill in the sfdc.username and sfdc.password with your credentials.

## Configure the Listener and SF connector

### Listener 
Configure the port and path

### Configure the Create job bulk api v 2
Configure salesforce connection
`Production/DE URL:
`Username: ${sfdc.username}
`Password: ${sfdc.password}

Configure properties
`Specify the 
`Object Type: Contact
`sObjects: payload
`Operation: upsert
`External id field name: Customer_Sequence_Number__c



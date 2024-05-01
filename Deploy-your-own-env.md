### Get started with deploying your Environment.

This document will help you deploy the Azure Open AI + Teams Bot Empowering Knowledge Workers lab envrionment in your Azure environment.To Deploy this lab in your env, Please follow the below steps;


1. You will need following to get started:

   - **OpenAI Resource**: Enable your subscription for OpenAI resource deployment. [here](https://aka.ms/oai/access).
   - **Azure subscription**: Create a free account [here](https://azure.microsoft.com/free/).
   - **Azure Permission**: Make sure you have owner Access to the Subscription. 

## Prepare your Azure Lab Environment.

1. Click on the below Deploy to Azure Button.

   [![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https://experienceazure.blob.core.windows.net/templates/azure-ai-ms-teams/opnai-deployment1.json)

   - Select the available subscription and resource group. Provide the unique alpha numeric value for `Deployment` parameter. You can review the ARM template by clicking on Edit Template. Review and create your lab envrionment.


Once All the resources got deployed, you can login to the JumpVM to perform the lab. 

# Azure OpenAI Workshop
## Empowering Knowledge Workers using Azure OpenAI & Microsoft Teams Bot (ITSM)

Welcome to the Azure OpenAI workshop! In this workshop, you will learn how to use the Azure OpenAI service to create an AI powered solution. You will get hands-on experience with the latest AI technologies and will learn how to use Azure OpenAI API.

Prerequisites
To fully participate in this workshop, you should have:

1. Basic understanding of AI and Machine Learning
2. Basic knowledge of Python Programming
3. An Azure account (sign up for a free trial if you don't have one already)
4. Access to Azure OpenAI service

## Structure
- teams-bot
- openai-model
  - data
  - notebooks
  - flask-app
  - outputs
  - config.py
  - requirements.txt
  - README.md

# Setting up Azure OpenAI Service

## Creating an OpenAI Resource in Azure

Azure resources can be created in several different ways, including within the Azure portal, using REST APIs, Azure CLI, PowerShell or client libraries, and via ARM templates. Here are the steps for creation of an OpenAI resource through the Azure portal.

## Steps

1. Navigate to the create page: [Azure OpenAI Service Create Page](https://portal.azure.com/?microsoft_azure_marketplace_ItemHideKey=microsoft_openai_tip#create/Microsoft.CognitiveServicesOpenAI).

2. On the Create page, provide the following information:

| Field         | Description                                                                                                     |
| ------------- | --------------------------------------------------------------------------------------------------------------- |
| Subscription  | Select the Azure subscription used in your OpenAI onboarding application.                                      |
| Resource group| The Azure resource group that will contain your OpenAI resource. You can create a new group or add it to a pre-existing group. |
| Region        | The location of your instance. Different locations may introduce latency, but have no impact on the runtime availability of your resource. |
| Name          | A descriptive name for your cognitive services resource. For example, MyOpenAIResource.                          |
| Pricing Tier  | Only 1 pricing tier is available for the service currently.                                                     |

![OpenAI Create Resource](https://learn.microsoft.com/en-us/azure/cognitive-services/openai/media/create-resource/create.png)

3. After you have provided all the information, click on the "Review + create" button.

4. Review your settings and then click on the "Create" button to create your OpenAI resource.

## Deploy a model
Before you can generate text or inference, you need to deploy a model. You can select from one of several available models in Azure OpenAI Studio.

Davinci is the most capable model family and can perform any task the other models can perform and often with less instruction. For applications requiring a lot of understanding of the content, like summarization for a specific audience and creative content generation, Davinci is going to produce the best results.

## To deploy a model, follow these steps:

1. Sign in to Azure OpenAI Studio.
2. Select the subscription and OpenAI resource to work with.
3. Select Manage deployments in your resource > Go to Deployments under Manage your deployments and models. You might first need to scroll down on the landing page.

![Screenshot of Azure OpenAI Studio page with the 'Go to Deployments' button highlighted.](https://learn.microsoft.com/en-us/azure/cognitive-services/openai/media/create-resource/deployment.png)

4. Select Create new deployment from the Management > Deployments page.
5. Select a model from the drop-down. For getting started in the East US region, we recommend the text-davinci-003 model. In other regions you should start with the text-davinci-002 model. Some models are not available in all regions. For a list of available models per region, see Model Summary table and region availability.
6. Enter a model name to help you identify the model. Choose a name carefully. The model name will be used as the deployment name via OpenAI client libraries and API.
7. Select Create to deploy the model.

The deployments table displays a new entry that corresponds to this newly created model. Your deployment status will move to succeeded when the deployment is complete and ready for use.

There are 3 labs in this workshop:

## Lab 1. Leveraging an OpenAI model to create extract data and create embeddings.
  - Install all the required libraries using requirements.txt file
  - Update the configuration file with newly generated credentials 
  - Experiment with notebooks to explore data and model 
  - Review all the modules

## Lab 2. Deploying the model using Flask framework locally and on Azure App Service. Setting up Email Automation Workflow on Azure Logic.
  - Deploy the model by running the Flask wrapper locally
  - Test the locally-deployed API with specified request/response formats
  - Deploy the model on Azure App Service
  - Test the cloud-deployed API with specified request/response formats
  - Setup email automation workflow on Azure Logic Apps using 

## Lab 3. Deploying the chatbot on Azure Bot Service and Azure App Service. 
  - Explore the chatbot codebase to understand user journey and dialogue development 
  - Update the configuration file with newly generated credentials 
  - Deploy the chatbot on Azure Bot Service and Azure App Service
  - Publish the chatbot on Microsoft Teams channel using a manifest file

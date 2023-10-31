# CHATBOT-PROJECT
Chatbot project(IBM)
by -Aneesha
# Create a banking chatbot with FAQ discovery, anger detection and natural language understanding
In this code pattern, we will create a chatbot using Node.js and Watson Assistant. The Assistant flow will detect customer emotions and be enhanced by using Natural Language Understanding to identify location entities. For FAQs, a call to the Discovery service will use passage retrieval to pull answers from a collection of documents.

When the reader has completed this pattern, they will understand how to:

* Create a chatbot that converses via a web UI using Watson Assistant and Node.js
* Use Watson Discovery with passage retrieval to find answers in FAQ documents
* Identify location entities with Watson Natural Language Understanding

NOTE: This code pattern has been updated to include instructions for accessing Watson services running on IBM Cloud Pak for Data. These updates can be found in the specific instructions for deploying your app locally, or deploying your app to OpenShift on IBM Cloud. The main change required is that your application will need additional credentials to access the IBM Cloud Pak for Data cluster that is hosting the Watson services.

Click here for more information about IBM Cloud Pak for Data.

architecture

# Flow
* The FAQ documents are added to the Discovery collection.
* The user interacts with a chatbot via the app UI.
* User input is processed with Natural Language Understanding (NLU). The context is enriched with NLU-detected entities and keywords (e.g., a location).
* The input and enriched context is sent to Assistant. Assistant recognizes intent, entities and dialog paths. It responds with a reply and/or action.
* Optionally, a requested action is performed by the app. This may include one of the following:
     Lookup additional information from bank services to append to the reply
     Use Discovery to reply with an answer from the FAQ documents
  
# Included components
* IBM Watson Assistant: Build, test and deploy a bot or virtual agent across mobile devices, messaging platforms, or even on a physical robot.
* IBM Watson Discovery: A cognitive search and content analytics engine for applications to identify patterns, trends, and actionable insights.
* IBM Watson Natural Language Understanding: Analyze text to extract meta-data from content such as concepts, entities, keywords, categories, sentiment, emotion, relations, semantic roles, using natural language 
  understanding.
  
# Featured technologies
Steps
1.Create Watson services
2.Customize the Watson Assistant skill
3.Use the facebbok meesanger and slack 
  
# 1. Create Watson services
Provision the following services:

*Watson Assistant
*Watson Discovery
*Watson Natural Language Understanding

NOTE: If you will be using the Deploy to Cloud Foundry on IBM Cloud deployment option, then you can skip these next steps and jump right to the Deploy the Application section. That deployment option automatically creates the services and links them to your application.

The instructions will depend on whether you are provisioning services using IBM Cloud Pak for Data or on IBM Cloud.

Click to expand one:

* IBM Cloud Pak for Data
* IBM Cloud

# 2. Customize the Watson Assistant skill
The following instructions will depend on if you are provisioning Assistant from IBM Cloud or from an IBM Cloud Pak for Data cluster. Choose one:

Provision on IBM Cloud Pak for Data
Provision on IBM Cloud
To find the Skill ID for Watson Assistant:

* Go back to the Skills tab.

* Click on the three dots in the upper right-hand corner of a card and select View API Details.

* Copy the Skill ID GUID. Use this value when setting up your run-time environment.

* By default the application will import and use the skill named watson-chatbot, but you can configure it to use another skill by setting the run-time environment variable SKILL_ID.
  
* To view the Assistant dialog, click on the skill and choose the Dialog tab. Here's a snippet of the dialog:
  
![Screenshot 2023-10-23 195201](https://github.com/Aneesha5008/CHATBOT-PROJECT/assets/144435424/2e34d946-bb18-468f-b395-b3d9e9513f57) 

# 3. Use the facebbok meesanger and slack


![Screenshot 2023-10-29 195104](https://github.com/Aneesha5008/CHATBOT-PROJECT/assets/144435424/b1513450-58e6-4e50-9f8e-0d449e571690)

![Screenshot 2023-10-29 195336](https://github.com/Aneesha5008/CHATBOT-PROJECT/assets/144435424/4380035a-6948-4ce9-9608-a4aae5adfd39)

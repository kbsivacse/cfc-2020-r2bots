# Community Hub – A collaboration channel 
Cognizant Resilinece & Reliability (R2) Engineering ™ team's submission for IBM Call for Code (CFC 2020) Hackathon.

## Overview
Communities need to cooperate among themselves to solve their needs in times of crisis, whether it be to advertise where supplies are held, offer assistance for collections, or other local services like volunteer deliveries. Many of the nations in the world need to lockdown their cities for prolonged duration to control the COVID-19 spread. People in the respective cities and communities run out of essential food, household and other supplies very quick. Their essential needs has to be full filled in secured manner with social distancing. 

This mobile application is for the people in need to find nearby supplies for their essential demands during crisis situations. It also provide a channel to offer voluntary services, donations to the needed communities. By using this application, communityies will be able to view,
1. Top demand and supplies in their localties
2. Lookup the supplies for their demands using chatbot 
3. Facility to post the vegetable stock by farmers/producers, voluntary service providers, locality needs of community people to see and respond

## Technology Stack

1. Reactive Native - UI
2. Node.js - API
3. IBM Cloudant - Database (No-SQL)
4. IBM Watson Assistant - Chat-bot
5. IBM Cloud - Cloud Foundary Services

## Logical flow
This solution has a chat interface built using IBM Watson Assistant, data storage to hold the status of demands and supplies available, and location services with real-time information to get users the information they need.

<img src="images/architecture-diagram.png"
     alt="architecture-diagram"
     style="float: left; margin-right: 10px;" />

1. The user in need/demand launches the mobile app and can access information across multiple services.
2. The user in need/demand can ask questions to virtual Assistant and get answers on food/service availability questions, top demands/supply, create a new demand/donation/supply.
3. The Supplier user can post the availability of resources they can provide, as well as locate the items they need.
4. The user in need/demand can obtain geolocation data to plot routes to collect (or drop off) supplies using HERE Location Services.

## IBM Cloud Services
IBM Cloud services provide an easy way of implementing the solution in short span of time using,
1. Application is developed using React Native for UI, Node.js for API layer with IBM Cloudant No-SQL database at the backend levaraging IBM's statrtup kit for the hackathon
2. Application is hosted as Cloud Foundary Services on IBM cloud
3. IBM Watson Assistan for Chatbot integration to post the demand and get nearby supplies with contact details as response. Chatbot also helps to add supplies and dontations by invoking backend Node.js API hosted

## Virtual Assistant
Virtual assistant developed using IBM Watson Assistant integrates with APIs to provide below support by using simple chat,

1. Lookup for top demand/supplies
2. Search for supplies available for specific product in need in sepecific locality
3. Create a new demand/supply/donation

Virtual assistant (standalone) for this application can be accessed [here](https://integrations.eu-gb.assistant.watson.cloud.ibm.com/web/public/e8da9e06-9785-4149-9ea2-9b19e908172b).

## Solution Roadmap
The basic featured and functionalties of the application is extended from IBM's CFC 2020 hackathon statrup kit. The chat-bot has been trained to respond dynamically based on user need and provide real-time accuracy in the response. It also helps to create demands or supplies for a brand new user by asking relevant questions. The below are some of the additional features that can be added to make this more relevant and better as a platform.

1. Search result based on distance using map APIs
2. Retail implementation to connect demand vs supplier
3. 3rd party login integration
4. Alerts via push notification or preferred communication channel
5. Chat with supplier or requester (one-to-one)
6. Voice enabled search

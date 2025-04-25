# AI Cockpit - Human on the loop

<img src="doc/chemistree_logo.svg" alt="Chemistree Logo" align="left" style="width:180px;float: left"/> In this field lab a AI Cockpit for "Human on the Loop" was developed assisting those who are assigned the role of “human oversight” under the AI Act to effectively monitor and control an AI system. 

The Software in this field lab was developed by [Chemistree GmbH](https://www.chemistree.de/).

## AI Cockpit Features

The AI Cockpit software solution is a web and API-based application that allows users to:

* specify and describe modules of an existing AI system
* associate multiple levels of autonomy for a module
* create and describe risks for the whole AI system or for specific modules
* create measures in order to monitor, reduce or eliminate the risks, e.g. key performance indicators
* visualize all key performance indicators in charts and define alarm zones for alerts
* have an overview of all measures on a single cockpit dashboard
* change the level of autonomy of individual modules
* press a stop button that navigates the AI system in defined levels of autonomy
* communicate with the AI system via an standardized API, that allows to import configuration data and reduce manual work
  
The AI Cockpit has been designed in a generic way so that it can be used by all industries, not just human resources, for which it was originally developed.

For more technical details have a look at our GitHub-Repository of the [AI Cockpit Human on the Loop](https://github.com/chmstr/ai-cockpit)

## AI-Cockpit API (KIC-API)

The AI-Cockpit communicates with a backend for persistent data. But the AI-Cockpit can also communicate directly with the AI-System itself, if the AI-System implements the given [AI-Cockpit API](https://github.com/chmstr/ai-cockpit/blob/main/api/kic-api-v1.0.0.yaml), which defines the basic use-cases for automatic configuration and control. The functionality of the API covers the following use cases:

* Set the active autonomy level for a specific module of an AI system
* Get the active autonomy level of a module
* List all autonomy levels of an AI module
* List all details including autonomy levels of a module
* List all modules with all details including autonomy levels
* Get labels and datasets of a key performance indicator

### Open Source

The developed solution is open source and uses mainly two other open source projects:

* [Vue.js](https://vuejs.org/): an open-source JavaScript framework specifically designed for building user interfaces (UIs) and single-page applications (SPAs).
* [Appwrite](https://appwrite.io/): an open-source self-hosted Backend-as-a-Service (BaaS) platform, used for Authentication, Databases, Functions, Storage, and Messaging.
  
The AI Cockpit of Chemistree is 100% open source and published under [AGPL V3](https://github.com/chmstr/ai-cockpit/blob/main/LICENSE).

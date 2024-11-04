# Azure AIML Implementation
> Welcome to my AI/ML project repository! Here, I share a suite of projects focused on applying Azure’s powerful AI and ML tools for model development, deployment, and data management. This space is crafted to offer insights, tools, and resources dedicated to enhancing understanding and integration of AIML in the cloud.

**1. Language Detection Using Azure Text Analytics API**
> This project serves as an introduction to AI/ML with Azure by leveraging the Text Analytics API to identify the language of user-provided text.

**Project Overview**
> In this Python-based project, we use the Azure Text Analytics API to analyze user-input text and return the detected language. This beginner-friendly project highlights basic cloud integration in the AIML domain.

**Requirements**
> Python Version: 3.x
> Libraries: dotenv, http.client, json
> Azure Service: Azure Text Analytics API, including an API endpoint and key.

**Setup Instructions**
> Clone the Repository: git clone https://github.com/yourusername/Azure_AIML_Implementation.git
> Install Dependencies: pip install python-dotenv
> Configure Environment Variables:
> Create a .env file with the following details: 
> AI_SERVICE_ENDPOINT=your_azure_endpoint
> AI_SERVICE_KEY=your_azure_key

**Usage**
> Run the script by executing: python script_name.py
> Enter any text to detect its language. Type "quit" to exit.

**Sample Output**
> For example, entering "Bonjour" will produce output similar to:
{
  "documents": [
    {
      "id": "1",
      "detectedLanguage": {
        "name": "French",
        "iso6391Name": "fr",
        "confidenceScore": 1.0
      }
    }
  ]
}
> Language: French

**Error Handling**
> Typical issues include:
> Authentication Errors: Caused by an invalid API key.
> Endpoint Errors: Result from an incorrect endpoint.


**2. Language Detection Using Azure Text Analytics Client SDK**
> This project enhances the previous one by using the Azure Text Analytics Client SDK for streamlined language detection.

**Project Overview**
> Using Python and the TextAnalyticsClient from Azure, this script allows users to input text, processes it through the Text Analytics service, and returns the detected language. This project is designed to further explore Azure’s cloud-based AI/ML services.

**Requirements**
> Python Version: 3.x
> Libraries: dotenv, azure-ai-textanalytics
> Azure Service: Requires endpoint URL and API key for the Text Analytics API.

**Setup Instructions**
> Clone the Repository: git clone https://github.com/yourusername/Azure_AIML_Implementation.git
> Install Dependencies: pip install python-dotenv azure-ai-textanalytics
> Configure Environment Variables:
> In the project directory, create a .env file and add: 
> AI_SERVICE_ENDPOINT=your_azure_endpoint
> AI_SERVICE_KEY=your_azure_key
> Input any text to identify its language. Type "quit" to end the session.

**Sample Output**
> Entering "Hola" might yield:
> Language: Spanish

**Error Handling**
> Common errors include:
> Authentication Issues: Caused by invalid API keys.
> Endpoint Errors: Occur if the endpoint URL is incorrect.

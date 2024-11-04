Language Detection with Azure Text Analytics API
This repository contains the first project in learning AI/ML with Azure. The project uses the Azure Text Analytics API to detect the language of user-input text.

Overview
This Python script sends text to Azure’s Text Analytics service, which returns the detected language. It’s an introductory project for understanding AI/ML integration in the cloud.

Requirements
Python 3.x
Libraries: dotenv, http.client, json
Azure Text Analytics API: Requires an Azure API endpoint and key.
Setup
Clone the repository:

bash
Copy code
git clone https://github.com/yourusername/Azur-aiml-implementation.git
Install dependencies:

bash
Copy code
pip install python-dotenv
Configure environment variables:

Create a .env file with:
env
Copy code
AI_SERVICE_ENDPOINT=your_azure_endpoint
AI_SERVICE_KEY=your_azure_key
Usage
Run the script:
bash
Copy code
python script_name.py
Enter text to detect its language; type "quit" to exit.
Sample Output
Entering "Bonjour" as input might produce:

json
Copy code
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

Language: French
Error Handling
Common errors include:

Authentication Error: Invalid API key.
Endpoint Error: Incorrect endpoint.

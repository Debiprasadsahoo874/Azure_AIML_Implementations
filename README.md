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


# Background Removal and Image Analysis with Azure Computer Vision
>  In this project, I explored Azure's Computer Vision service to analyze images and perform background removal or foreground extraction using Python. The project showcases how to leverage Azure’s Computer Vision API for practical applications, from feature detection to background removal.

**Overview**
> This Python script connects to Azure's Computer Vision API to:
> Analyze an image to retrieve specific features such as captions, tags, and objects.
> Perform background removal or create a foreground matte for image enhancement.
> This project is part of an ongoing series aimed at exploring Azure AI/ML capabilities and integrating cloud-based computer vision.

**Features**
> Image Analysis: Retrieves captions, tags, objects, and people detection from an image.
> Background Removal: Option to remove the background or isolate the foreground for visual clarity.

**Requirements**
> Python 3.x
> Libraries: dotenv, Pillow (PIL), matplotlib, requests, azure.core.exceptions
> Azure Computer Vision API: Requires an endpoint URL and API key from Azure.

**Setup Instructions**
> 1. Clone the repository:git clone https://github.com/Debiprasadsahoo874/Azure_AIML_Implementations.git
cd Azure_AIML_Implementations
> 2. Install Dependencies: pip install python-dotenv Pillow matplotlib requests azure-core
> 3. Configure Environment Variables:
> Create a .env file in the project directory and add your Azure API endpoint and key:
> AI_SERVICE_ENDPOINT=your_azure_endpoint
> AI_SERVICE_KEY=your_azure_key
> 4. Add an Image: Place an image named street.jpg in an images folder, or provide the file path as a command-line argument when running the script.

**Usage**
> Run the script to analyze the image and optionally remove the background: python Background_removal_and_image_analysis.py
> Alternatively, specify a different image file: python Background_removal_and_image_analysis.py images/your_image.jpg

**Sample Output**
> Analyzed Image Features: The script outputs captions, dense captions, tags, detected objects, and people.
> Background Removal: Saves an image with the background removed or the foreground isolated.

**Error Handling**
> Common errors include:
> Authentication Error: Check your API key.
> HTTP Response Error: Verify image format and endpoint configurations.


# Azure AI Vision Text Reader
> This project uses the Azure AI Vision SDK to read text from images, including options for printed and handwritten text. It demonstrates setting up an Azure Vision client to analyze images, extract text, and highlight detected text directly on the image.

**Features**
> Text Extraction: Leverages the Azure AI Vision SDK to detect and read text from images, supporting both printed and handwritten text.
> Bounding Polygon Visualization: Highlights text and bounding polygons around each detected word or line within the image.
> User Options: A menu-driven interface allows users to select different images for analysis.

**Overview**
> This project showcases Azure's AI and machine learning capabilities for Optical Character Recognition (OCR), enabling cloud-based text extraction, even for Indian languages.

**Requirements**
> Python 3.x
> Libraries: dotenv, requests, azure.core.exceptions
> Azure AI Vision API: Requires an endpoint URL and API key for access

**Setup**
> 1. Clone the Repository: https://github.com/Debiprasadsahoo874/Azure_AIML_Implementations/blob/main/Image_text_detector.py
> 2. Install Dependencies: pip install python-dotenv requests azure-core
> 3. Configure Environment Variables- Create a .env file in the project directory with the following contents:
>    AI_SERVICE_ENDPOINT=your_azure_endpoint
>    AI_SERVICE_KEY=your_azure_key
> 4. Add an Image File: Place an image with text in the images folder, or specify the path to a different image file for processing.

**Usage**
> Run the Script: python text_reader.py
> Specify a Different Image File: python text_reader.py images/your_image.jpg

**Sample Output**
> Console Output: The extracted text is displayed in the console.
> File Output: The text is saved as a .txt file in the project directory.
> Bounding Polygon Visualization: The processed image, with highlighted bounding boxes around detected text, is saved as text.jpg.

**Error Handling**
> Authentication Errors: Ensure the API key is valid and properly configured in the .env file.
> HTTP Response Errors: Check for supported image formats and verify the endpoint configurations.

**License**
> This project is open-sourced under the MIT License.

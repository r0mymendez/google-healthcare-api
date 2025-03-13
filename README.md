[![Buy Me A Coffee](https://img.shields.io/badge/Buy%20Me%20A%20Coffee-support%20my%20work-FFDD00?style=flat&labelColor=101010&logo=buy-me-a-coffee&logoColor=white)](https://www.buymeacoffee.com/r0mymendez)

---

# ☁️ Healthcare Natural Language API - (PoC)

## Project Overview

This project is a Proof of Concept (PoC) using Google Cloud's Healthcare Natural Language API. The goal is to test the API's ability to extract medical entities and relationships from unstructured clinical notes, leveraging pre-trained natural language models.

![img](img/image-api-google.webp)


## About Healthcare Natural Language API

The Healthcare Natural Language API is part of the Google Cloud Healthcare API. It uses natural language processing (NLP) models to extract healthcare-related information from medical text.

### Key Features

The API can identify and extract:

- 🏥 **Medical concepts** such as medications, procedures, and health conditions.
- 📅 **Functional attributes** like temporal relationships, subjects, and certainty assessments.
- 🔗 **Relationships** between entities, such as side effects or drug dosages.

### Core Functionality

In this tutorial, we will focus on the following function:

- **Entity Analysis**: The `analyzeEntities` method inspects medical text to detect and return medical concepts and their relationships.

## Prerequisites

Before running this PoC, ensure you have completed the following steps:

1. ✅ **Google Cloud account**: You must have a Google Cloud account set up.
2. 🌐 **Enable APIs**: Ensure the Cloud Healthcare API and Healthcare Natural Language API are enabled.
3. 🛠️ **Install Google Cloud CLI (gcloud)**: Download and install the Google Cloud CLI.
4. 📄 **Create a `.env` file**: This file will store the necessary environment variables.

### Create a `.env` file

To configure the environment variables, create a `.env` file in your project directory and add the following content:

```
PROJECT_ID = "project_name"
LOCATION = "location_name"
TOKEN = "token_value"
```

### How to obtain the token value

Follow these steps to authenticate and get your access token:

1. **Authenticate with Google Cloud** by running the following command in your terminal:

```
gcloud auth login
```

2. **Get the access token** by running:

```
gcloud auth print-access-token
```

Copy the token value and paste it into the `.env` file under the `TOKEN` variable.

## Goals

- Test entity extraction from clinical notes.
- Evaluate how well the API identifies medical concepts and maps relationships.
- Understand the output format and how to integrate the extracted data into a larger cloud architecture.

## Next Steps

1. Set up Google Cloud Healthcare API.
2. Enable the Healthcare Natural Language API.
3. Implement entity analysis using the `analyzeEntities` method.
4. Analyze the results and review entity mapping.

----

⚠️ **Important Note:** The medical note included in this repository is entirely fictitious. It was generated for a fictional healthcare professional and does not belong to any real patient. This data is solely for testing and demonstration purposes.


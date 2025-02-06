# AI Chat Deployment Guide

This repository provides the necessary steps to set up and test this AI chat that uses Bubble.io and n8n. Follow the steps below to do it.

## 1. **Duplicate the Bubble.io Project**

To duplicate the project I’ve created in Bubble.io, follow these steps:

### Step 1: Duplicate the Bubble.io Project
1. **Access the Bubble.io Project**
   - Go to https://alvarodzglez.bubbleapps.io.
   - Locate the project you want to duplicate.

2. **Duplicate the Project**

3. **Set Up the Duplicated Project**
   - Once duplicated, open the copied project.
   - Ensure the system is functioning as expected by reviewing the workflows, database, and design.

4. **Deploy the Project**
   - Click on the **"Launch"** button to deploy the chat system.
   - After deployment, copy the URL of the live chat system and share it for testing.

---

## 2. **Set Up n8n Workflow Automation**

This system uses n8n for workflow automation. Follow the steps to import and configure your n8n workflow.

### Step 1: Import the n8n Workflow JSON
1. **Access your n8n instance**:
   - If you don’t have an n8n account, create one.

2. **Import the JSON Workflow**:
   - Download the `Handling_API_call_to_OpenAI.json` file from this repository.
   - In your n8n instance, go to the **"Create Workflow"** section.
   - Search the settings button and click **"Import from File..."** and upload the `Handling_API_call_to_OpenAI.json` file.

3. **Review and Update API Key**:
   - Once the workflow is imported, open the workflow editor on **"Editor"** window.
   - Find the HTTP Request node.
   - Replace `API_KEY` in this node with your actual OpenAI API key.
   - Ensure that all other configuration settings are correct according to your system needs.

4. **Test the Workflow**:
   - After importing and updating the workflow, test the workflow on **"Executions"** window.
   - Ensure that the automation works as expected by sending messages through Bubble.io and verifying that n8n processes the data correctly.

---

## 3. **Repository Contents**

This GitHub repository contains the following files:

- **README.md** – This file, providing setup and test instructions.
- **n8n Workflow JSON** – The exported JSON file for the n8n workflow.
- **Screenshots** – Visual documentation of the Bubble.io UI and n8n automation.

---

## 4. **Testing the System**

To test the system:

1. Ensure the chat system is deployed and accessible via the Bubble.io link.
2. Import the n8n workflow JSON into your n8n instance.
3. Replace `API_KEY` in the workflow with your actual OpenAI API key.
4. Run the workflow and test the functionality by sending messages through the chat system.
5. Ensure that automated actions (e.g., replies, triggers) are working as expected.

---

## 5. **Screenshots and Documentation**

You will find screenshots of the Bubble.io UI and the n8n workflow within the repository.



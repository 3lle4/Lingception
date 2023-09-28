# Lingception: Using Natural Language Engineering to Explain Natural Language Engineering.

This is the bot for the project "Lingception" by Ellena Nett and Annika Traßl-Wilterius. It investigates to what extent contextualization of ChatGPT with a PDF improves the reliability of answers to questions about the given context. The architecture of the bot is based on the work of mayooear and this repo [gpt4-pdf-chatbot-langchain](https://github.com/mayooear/gpt4-pdf-chatbot-langchain/tree/feat/vectordbqa). (Frontend of this repo is inspired by [langchain-chat-nextjs](https://github.com/zahidkhawaja/langchain-chat-nextjs))

The setup describes the steps to start the bot locally and connect to already used API. The complete setup incl. ingestion of a PDF can be found in the origin repo.

## Set up the bot

1.	Install packages

First run `npm install yarn -g` to install yarn globally.

Then run:

```
yarn install
```
After installation, there should be a `node_modules` folder.

2.	Set up the `.env` file

-	Copy `.env.example` into `.env`
The `.env` file should look like this:

```
OPENAI_API_KEY=

PINECONE_API_KEY=
PINECONE_ENVIRONMENT=

PINECONE_INDEX_NAME=

```
-	enter the APIs
-	enter pinecone parameter

## Run the app

Run the app `npm run dev` to launch the local dev environment, and then type a NLP question in the chat interface.


# Day 3 – HackMate AI: Hackathon & Student Events Assistant

## Project Overview
HackMate AI is an AI-powered assistant designed to help students and volunteers with hackathon coordination, college events, team communication, and registration-related queries.

It uses Google's Gemini API and LangChain to provide helpful responses and generate professional WhatsApp messages for event coordination.

## Objectives
- Build an AI-powered hackathon coordination assistant.
- Integrate the Gemini API using LangChain.
- Answer student and volunteer queries.
- Generate polite WhatsApp reminders for team leads.
- Maintain conversation history.
- Test AI responses using CSV test cases.
- Create a basic LangChain agent.

## Technologies Used
- Python
- Google Colab
- Google Gemini API
- LangChain
- langchain-google-genai
- CSV

## Implementation
1. Installed the required Python libraries.
2. Configured the Gemini API key securely using Google Colab Secrets.
3. Connected to Gemini using `ChatGoogleGenerativeAI`.
4. Selected the `gemini-3.8-flash` model.
5. Created a system prompt defining the HackMate AI assistant's role and instructions.
6. Developed a prompt template using `ChatPromptTemplate` and `MessagesPlaceholder`.
7. Created a LangChain chain using `StrOutputParser`.
8. Implemented conversation history to maintain previous messages.
9. Created CSV-based testing using `test.csv`.
10. Developed a basic AI agent using LangChain's `create_agent`.

## Key Features
- Hackathon team coordination assistance.
- Shortlisting email confirmation message drafts.
- Payment deadline reminder drafts.
- Student event and club query assistance.
- Conversation history.
- CSV-based response testing.
- AI agent interaction.

## Sample Questions
1. What can you help me with as a hackathon volunteer?
2. Draft a WhatsApp message asking a team lead to confirm receipt of the shortlisting email.
3. Write a polite payment deadline reminder.
4. A team is not interested in participating. How should I record this response?
5. What is the event venue?

## API Configuration
The Gemini API key is stored securely in Google Colab Secrets and accessed through the `userdata` module.

The API key is not hardcoded in the notebook.

## Learning Outcomes
- Learned Gemini API integration with LangChain.
- Understood prompt templates and system instructions.
- Implemented conversation history.
- Practiced CSV-based testing.
- Learned to create a basic LangChain agent.
- Understood secure API key management.

## Challenges
- Resolved Gemini API secret-name configuration.
- Installed the required LangChain Gemini integration package.
- Updated the model name based on API availability.
- Encountered temporary Gemini server-side 503 high-demand errors and used retry handling.

## Status
**Day 3 – Implementation completed; testing may require retries during Gemini service unavailability.**
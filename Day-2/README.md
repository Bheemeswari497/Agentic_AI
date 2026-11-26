# Day 2 – UniFest AI: Events & Clubs Assistant

## Project Overview
UniFest AI is an AI-powered Events and Clubs Assistant designed to help students get information about college events, technical fests, coding contests, and student clubs through a simple chat interface.

## Objectives
- Build an AI-powered college events assistant.
- Connect to the Groq API using an OpenAI-compatible client.
- Answer student queries about events and clubs.
- Create an interactive chatbot interface using Gradio/HTML widgets.

## Technologies Used
- Python
- Google Colab
- Groq API
- OpenAI Python Library
- Google Colab Secrets
- IPython Widgets

## Implementation
1. Installed and imported the required Python libraries.
2. Retrieved the Groq API key securely using Google Colab Secrets.
3. Connected to the Groq API using the OpenAI-compatible client.
4. Configured the model `openai/gpt-oss-120b`.
5. Developed the UniFest AI Events & Clubs Assistant.
6. Created an interactive chat interface with Send and Reset Chat options.
7. Tested the chatbot using sample questions.

## Sample Questions
1. When is the InnovateX Tech Fest?
2. Where will the coding contest take place?
3. How can I register for an event?
4. What is the registration deadline?
5. When does the RoboSphere Club meet?

## Sample Output
- Greeting: The assistant responds to student greetings.
- Event Information: Provides details about InnovateX Tech Fest.
- Venue Information: Displays the event location when asked.
- Chat Interface: Allows students to interact with the assistant.

## API Configuration
The Groq API key is stored securely in Google Colab Secrets and accessed using the `userdata` module. The API key is not hardcoded in the notebook.

## Learning Outcomes
- Learned how to connect Python applications with the Groq API.
- Understood OpenAI-compatible API integration.
- Learned how to build an AI-powered chatbot.
- Practiced creating interactive chat interfaces.
- Understood secure API key management.

## Status
**Completed – Day 2**
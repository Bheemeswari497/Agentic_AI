# Day 4 – HackMate AI: Team Coordination Agent

## Project Overview
HackMate AI is an AI-powered Hackathon Team Coordination Assistant designed to help organizers manage team information, track payment and participation status, draft reminders, and save verified team records.

The project uses Google Gemini and Google Sheets to support team coordination tasks.

## Objective
- Convert Python functions into AI agent tools using `@tool`.
- Create structured team records using Pydantic.
- Extract useful information from messy team messages.
- Store team details in Google Sheets.
- Test how the agent selects tools and handles tool calls.

## Technologies Used
- Python
- Google Gemini API
- LangChain
- LangChain Google GenAI
- Pydantic
- Google Colab
- Google Sheets
- gspread
- CSV

## Main Features

### 1. Hackathon Team Management
Find team details using the team ID and retrieve available team status information.

### 2. Payment Reminder Generation
Generate polite WhatsApp payment reminders for team leaders using the provided deadline and team details.

### 3. Structured Team Records
Use a Pydantic model to organize team information such as:
- Team ID
- Team name
- Team leader
- Email status
- Payment status
- Participation status
- Deadline
- Notes

### 4. Google Sheets Integration
Connect the HackMate AI agent to the `HackMate_Team_Tracker` Google Sheet to store verified team records.

### 5. CSV Message Processing
Use `team_messages.csv` as an input file for team-related messages and information.

### 6. Tool Calling and Trace Analysis
Explore tool selection, tool naming, model calls, and tool-call traces.

## Google Sheet
**Sheet Name:** HackMate_Team_Tracker

The sheet contains the following columns:

`team_id | team_name | team_lead | email_status | payment_status | participation_status | deadline | notes`

## Project Files

```text
Day-4/
├── Task4.py
├── team_messages.csv
└── README.md
```

## API Key Configuration

The Gemini API key is stored securely in Google Colab Secrets.

Secret name:

`GEMINI_API_KEY`

The API key is loaded using:

```python
from google.colab import userdata

api_key = userdata.get("GEMINI_API_KEY")
```

**Security:** API keys must not be committed to GitHub.

## Testing Status

- Gemini API connection: Successful.
- Google Sheets conversion: Completed.
- Google Sheets authentication and write integration: Testing.
- Final end-to-end agent testing: Pending due to Gemini free-tier daily quota exhaustion.

## Learning Outcomes
- Understanding AI agent tool calling.
- Creating structured outputs with Pydantic.
- Integrating Gemini with LangChain.
- Connecting Python applications to Google Sheets.
- Processing team coordination data.
- Understanding agent execution traces.

## Conclusion
HackMate AI demonstrates how an AI agent can simplify hackathon team coordination by organizing team information, generating reminders, and maintaining structured records using Google Sheets.

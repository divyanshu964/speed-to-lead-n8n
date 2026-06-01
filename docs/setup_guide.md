# Setup Guide

## Prerequisites
- n8n instance (self-hosted or cloud)
- Groq API key (free at console.groq.com)
- Gmail account with App Password
- Google Sheets
- Tally.so account

## Steps

1. Import `workflow.json` into your n8n instance
2. Create a Tally form with these fields:
   - First Name, Last Name, Work Email
   - Company Name, Company Size (dropdown)
   - Biggest Sales Challenge (textarea)
3. Connect your Groq API key to the HTTP Request nodes
4. Connect your Gmail account via OAuth2
5. Create a Google Sheet with headers matching the workflow
6. Update the Tally webhook URL to your n8n webhook URL
7. Publish the workflow

## Customization

- Change `LeadFlow CRM` to your client's company name
- Update the Calendly link in email prompts
- Adjust lead scoring thresholds in the Code node
- Modify email tone in the system prompt

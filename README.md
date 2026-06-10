# AI Email Triage System — Automated Classification & Routing

An intelligent email triage system that automatically reads, 
classifies, and routes incoming emails to the correct 
department — eliminating manual inbox sorting entirely.

## Problem It Solves
Businesses receiving high volumes of emails were spending 
hours manually reading and forwarding messages to the right 
teams. Important emails were delayed, misrouted, or missed 
completely.

## Tools Used
- n8n (workflow automation)
- Gmail Trigger (email capture)
- OpenAI API (email classification)
- Switch node (department routing)
- Gmail (department-specific sending)
- Google Sheets (email log)

## How It Works
1. Gmail Trigger fires when a new email arrives in the inbox
2. Email subject and body are passed to OpenAI for classification
3. OpenAI returns a category:
   - Sales enquiry
   - Support request
   - Billing issue
   - General enquiry
4. Switch node routes based on OpenAI's classification
5. Email is automatically forwarded to the correct 
   department Gmail address
6. All emails and their classifications are logged 
   to Google Sheets for reporting

## Key Concepts Demonstrated
- Gmail Trigger → OpenAI → Switch node pipeline
- AI-powered text classification
- Multi-branch department routing
- Automated email forwarding
- Google Sheets audit logging

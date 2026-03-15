AI Account Intelligence & Enrichment System

Overview

This project is an AI-powered automation system that converts anonymous website visitor signals into structured account intelligence for sales teams.

It enriches visitor data using IP intelligence and AI analysis to identify companies, estimate buying intent, and generate recommended sales actions.

Built With
	•	n8n workflow automation
	•	OpenAI GPT models
	•	IP enrichment API
	•	Google Sheets CRM
	•	Slack alerts
	•	Gmail notifications

Workflow

Visitor Signals
↓
Webhook Input
↓
Normalize Input
↓
IP Enrichment
↓
AI Account Intelligence Agent
↓
Intent Scoring
↓
Sales Intelligence Output
↓
CRM + Alerts

Example Input# 
{
  "visitorId": "008",
  "companyName": "Rocket Mortgage",
  "domain": "rocketmortgage.com",
  "pagesVisited": ["/pricing", "/demo", "/contact", "/case-studies"],
  "timeOnSite": "8m 30s",
  "visitsThisWeek": 5,
  "referralSource": "linkedin",
  "deviceType": "desktop",
  "location": "Detroit, USA"
}

Example Output
{
    
"Company Name": 
"Rocket Mortgage",
  
"Website / Domain": 
"rocketmortgage.com",
   
"Industry": 
"Financial Services",
    
"Company Size": 
"2001-5000",
   
"Headquarters": 
"Detroit, USA",
   
"Likely Persona": 
"Mortgage Executive",
   
"Intent Score": 
"9 / 10",
   
"Intent Stage": 
"Evaluation",
    
"AI Summary": 
"Visitor identified as a high-potential prospect from Rocket Mortgage, displaying significant engagement with key content related to pricing and demos.",
    
"Recommended Sales Action": 
"Follow up with personalized email addressing mortgage solutions. | Schedule a demo with the sales team to discuss specific needs. | Provide case studies relevant to the mortgage industry."
  
}
Setup
	1.	Install n8n
	2.	Import the workflow JSON file
	3.	Add API credentials for:
	•	OpenAI
	•	Slack
	•	Gmail
	•	Google Sheets
	4.	Run the webhook endpoint

  POST /webhook/account-intelligence

  Demo Video

  https://www.loom.com/share/2343aba44a5d47268db8213e45cc3124
  
Author
Shashidhar Genna

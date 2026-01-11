# email_classifier_using_n8n

[![n8n](https://img.shields.io/badge/built_with-n8n-green)](https://n8n.io)

AI-powered Gmail sorter that automatically classifies emails into **Job Applications**, **Scholarships (Academic)**, or **Others** using OpenAI GPT-4.1-mini, then applies the matching Gmail labels to keep your inbox organized.

## What It Does

- Monitors Gmail inbox every minute for new emails
- Uses AI to classify email content into customizable categories
- Automatically applies correct Gmail labels based on classification
- Perfect for researchers, job hunters, and scholarship applicants tracking opportunities

## How It Works

Gmail Trigger (every minute) → OpenAI Text Classifier (GPT-4.1-mini) → Add Gmail Labels (Job/Scholarship/Others)

## 5-Minute Setup

1. **Import** `email_classifier.json` into your n8n instance
2. **Configure Gmail OAuth2** credentials (Trigger + 3 Label nodes) 
3. **Update Label IDs** in the 3 "Add label" nodes:
- Job Applications: Label_8701051501519091711 → Replace with YOUR ID
- Scholarships: Label_2115922346108373658 → Replace with YOUR ID
- Others: Label_2015993182768288832 → Replace with YOUR ID
5. **Add OpenAI API** credentials (works with n8n free credits)
6. **Activate** workflow

## 🛠️ Fully Customizable

**Change Categories Anytime:**
```json
Edit Text Classifier node → categories array:
{
"category": "Job Applications" → "PhD Programs",
"category": "Scholarships" → "Conference Invites", 
"category": "Others" → "Networking"
}



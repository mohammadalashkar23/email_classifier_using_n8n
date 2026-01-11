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




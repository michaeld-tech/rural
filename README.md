# Salvia AI

AI-powered health guidance for underserved communities.

## The Problem

In many rural and low-resource settings, people face serious delays before getting medical help.  
Common barriers include:

- Long travel time to clinics and hospitals
- Low doctor-to-patient ratios
- Limited access to trusted health information
- Language and literacy barriers
- Late response to emergencies due to uncertainty

These gaps can turn manageable symptoms into severe outcomes.

## Our Solution

Salvia AI is a mobile-first health guidance platform designed to help people take safer, faster action.

Core capabilities:

- **AI Health Chat**: users describe symptoms and receive structured, urgency-aware guidance
- **Urgency classification**: responses are labeled for home care, clinic visit, or emergency action
- **First Aid Guide**: step-by-step instructions for common and emergency situations
- **Regional outbreak alerts**: location-relevant health risk updates
- **Caregiver discovery**: nearby clinics, NGOs, community health workers, and hotlines
- **WhatsApp bot integration**: extends access through familiar messaging channels
- **Multilingual support**: localized experiences across multiple languages

## How Claude Is Used

Claude powers the conversational intelligence behind Salvia AI.

- On each user message, Claude analyzes symptoms and context
- It asks clarifying questions when information is incomplete
- It returns practical guidance in clear, low-jargon language
- It applies safety rules (no definitive diagnosis, no unsafe medication dosing)
- It formats responses to include urgency classification for rapid triage

Claude is used as a guidance engine, not a replacement for professional medical care.

## Impact We Aim For

Salvia AI is built to improve first-response healthcare decisions where access is hardest.

Our impact goals:

- Reduce harmful delays in seeking care
- Improve early identification of emergency warning signs
- Increase access to understandable health guidance in local languages
- Support frontline and community-based care pathways
- Help underserved populations reach the right care level faster

## Tech Overview

- **Frontend**: React + Vite
- **Backend**: Node.js + Express
- **Database**: MongoDB
- **Authentication**: JWT + Google OAuth
- **Messaging**: Twilio WhatsApp integration
- **AI**: Anthropic Claude API

## Local Development

### 1) Install dependencies

```bash
npm install
cd server && npm install
```

### 2) Configure environment

Create `server/.env` and set required values:

- `MONGODB_URI`
- `JWT_SECRET`
- `SESSION_SECRET`
- `CLIENT_URL`
- `GOOGLE_CLIENT_ID`
- `GOOGLE_CLIENT_SECRET`
- `GOOGLE_CALLBACK_URL`
- `TWILIO_ACCOUNT_SID`
- `TWILIO_AUTH_TOKEN`
- `TWILIO_WHATSAPP_NUMBER`
- `ANTHROPIC_API_KEY`

Set frontend environment variable:

- `VITE_API_URL`

### 3) Run app

Frontend:

```bash
npm run dev
```

Backend (new terminal):

```bash
cd server
npm run dev
```

## Disclaimer

Salvia AI provides educational guidance only and does **not** replace licensed medical professionals.  
For severe or worsening symptoms, users should seek immediate medical care.

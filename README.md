# 🤖 AI Travel Booking Assistant (n8n)

An **AI-powered Travel Booking Assistant** built using **n8n**, **Telegram**, and **Google Gemini**.
This project supports **text and voice-based conversations**, intelligently gathers travel details,
confirms bookings, creates **Google Calendar events**, sends **email confirmations**, and handles
**cancellation requests** automatically.

---

## ✨ Features

- 💬 Telegram Bot interface (Text + Voice)
- 🎙️ Voice-to-text transcription using AI
- 🧠 Conversational AI Agent (Google Gemini + LangChain)
- 🧾 Structured JSON-based booking extraction
- 📅 Google Calendar event creation
- 📧 Booking confirmation via email
- ❌ Cancellation request handling
- 🧠 Session-based conversation memory

---

## 🏗️ Workflow Architecture

Telegram Trigger  
→ Message Type Router (Text / Voice / Cancel)  
→ AI Travel Agent  
→ Booking Data Extraction  
→ Calendar Event Creation  
→ Email Confirmation  
→ Telegram Confirmation  

---

## 🧠 Booking JSON Schema

```json
{
  "destination": "Paris",
  "start_date": "2025-02-10",
  "end_date": "2025-02-15",
  "travelers": 2,
  "budget_level": "medium",
  "budget_amount": 3000,
  "transport_type": "flight",
  "hotel_type": "4-star",
  "food_preferences": "vegetarian",
  "email": "user@example.com",
  "special_requests": "None",
  "booking_complete": true
}
```

---

## 🛠️ Tech Stack

| Layer | Technology |
|-----|-----------|
| Automation | n8n |
| Messaging | Telegram Bot API |
| AI Model | Google Gemini |
| Agent Framework | LangChain |
| Speech-to-Text | OpenRouter |
| Calendar | Google Calendar API |
| Email | Gmail API |
| Language | JavaScript |

---

## ⚙️ Setup Instructions

### Prerequisites
- n8n (Cloud or Self-hosted)
- Telegram Bot Token
- Google Gemini API Key
- Google Calendar OAuth
- Gmail OAuth
- OpenRouter API Key

### Steps
1. Import the workflow JSON into n8n
2. Configure required credentials
3. Activate the workflow
4. Start chatting with your Telegram bot

---

## 💬 Usage

- **Book a trip**: “I want to travel to Bali for 5 days”
- **Voice booking**: Send a voice message
- **Cancel booking**: Send `cancel`

---

## 🔐 Security

- OAuth-based authentication
- No hardcoded secrets
- Session-isolated user memory

---

## 🚀 Future Enhancements

- Payment gateway integration
- Database storage (Supabase / Firebase)
- Admin dashboard
- PDF itinerary generation
- WhatsApp integration

---

## 👨‍💻 Author

**Tharanidharane V**  
Built using n8n and AI Agents

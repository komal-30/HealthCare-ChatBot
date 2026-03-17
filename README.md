# 🏥 AI Healthcare ChatBot

An intelligent conversational chatbot built using Google Dialogflow to provide healthcare assistance, COVID-19 information, appointment scheduling, and medical guidance during the pandemic.

---

## 📌 About

The AI Healthcare ChatBot is a conversational AI solution designed to address healthcare challenges during the COVID-19 pandemic. The chatbot provides real-time information about COVID-19 statistics, symptoms, preventive measures, appointment scheduling with doctors, and helpdesk support. Built on Google Dialogflow using Natural Language Processing, it delivers intelligent responses to patient queries and guides users through various healthcare options.

**Key Features:**
- COVID-19 statistics and analysis
- Appointment booking with doctors
- FAQ for health-related queries
- Helpdesk support and contact information
- Live news updates about COVID-19
- COVID-19 testing and treatment information

---

## 🛠️ Technology Stack

| Platform | NLP & AI | Configuration | Integration |
|:---:|:---:|:---:|:---:|
| Google Dialogflow | Intent Recognition | JSON Files | Telegram |
| Dialogflow Console | Entity Extraction | Agent Config | Messaging API |
| Machine Learning | Parameter Mapping | Intent Definitions | Web Chat Interface |
| Natural Language Processing | Small Talk Responses | Entity Mapping | User Communication |

---

## 📂 Project Structure

```
Healthcare-ChatBot/
├── entities/                          # Entity definitions
│   ├── AppointmentType.json          # Appointment types
│   ├── sys.geo-country.json          # Country entities
│   └── sys.geo-country_entries_en.json # Country entries
├── intents/                           # Intent definitions
│   ├── covid-info.json               # COVID-19 information
│   ├── appointment.json              # Doctor appointment
│   ├── faq.json                      # Frequently asked questions
│   ├── helpdesk.json                 # Support assistance
│   └── small-talk.json               # Casual conversations
├── agent.json                         # Agent configuration
├── customSmalltalkResponses_en.json  # Chatbot responses
├── package.json                       # Project metadata
├── Abstract.md                        # Project abstract
├── Report.md                          # Detailed project report
└── README.md                          # Project documentation
```

---

## 🚀 Quick Start

### Prerequisites
- Google account for Dialogflow access
- Telegram account (for chatbot integration)
- Basic understanding of NLP concepts

### Setup Instructions

1. **Access Dialogflow Console**
   - Go to https://dialogflow.cloud.google.com/
   - Create a new agent named "HealthCare-ChatBot"
   - Select language: English

2. **Import Entities**
   - Navigate to Entities section
   - Upload entity files from `entities/` folder:
     - AppointmentType.json
     - sys.geo-country.json
     - sys.geo-country_entries_en.json

3. **Import Intents**
   - Go to Intents section
   - Upload all intent JSON files from `intents/` folder
   - Each intent contains training phrases and responses

4. **Configure Agent**
   - Upload `agent.json` for agent configuration
   - Import `customSmalltalkResponses_en.json` for custom responses
   - Enable small talk for casual conversations

5. **Setup Telegram Integration**
   - Create Telegram bot via BotFather (@BotFather)
   - Get bot token from Telegram
   - Configure webhook in Dialogflow integration settings
   - Connect Telegram token to Dialogflow

6. **Deploy & Test**
   - Click "Build" in Dialogflow console
   - Test chatbot in Telegram messenger
   - Verify all intents and responses work correctly

---

## 💬 Chatbot Features

| Feature | Description |
|---------|-------------|
| **COVID-19 Stats** | Country, state, and district-wise COVID statistics |
| **Appointment Booking** | Schedule appointments with doctors |
| **FAQ** | Symptoms, precautionary measures, treatment info |
| **Help Desk** | Government helpdesk contact information |
| **Live News** | Real-time COVID-19 news updates |
| **Testing & Treatment** | Information about COVID testing and vaccines |
| **Small Talk** | Natural conversational responses |

---

## 🎯 Use Cases

| Use Case | Description |
|----------|-------------|
| **Symptom Checker** | Users describe symptoms and get guidance |
| **COVID-19 Information** | Real-time statistics and pandemic data |
| **Doctor Appointments** | Book medical consultations |
| **Health FAQs** | Get answers to common health questions |
| **Emergency Support** | Quick access to helpdesk information |
| **Medical Guidance** | Information about treatments and prevention |
| **News Updates** | Stay informed about COVID-19 developments |

---

## 🔑 Key Dialogflow Concepts

**Intents** - User intentions mapped to responses
- Example: "I have a fever" → Symptom checker intent

**Entities** - Extract specific information from user input
- Example: AppointmentType entity (consultation, testing, vaccination)

**Actions & Parameters** - Link extracted data to responses
- Example: Extract doctor name, date, time for appointment booking

**Small Talk** - Natural conversation handling
- Example: Greetings, thanks, general questions with predefined responses

---

## 📈 Future Enhancements

- [ ] 🏥 Integration with online medical stores
- [ ] 💊 Medicine ordering and delivery
- [ ] 👨‍⚕️ Doctor profile database by location
- [ ] 🔍 Multi-disease symptom checker
- [ ] 🏡 Home remedies suggestions
- [ ] 📊 Health analytics dashboard

---


## 🔗 Resources

- [Google Dialogflow Documentation](https://cloud.google.com/dialogflow/docs)
- [Dialogflow Console](https://dialogflow.cloud.google.com/)
- [Telegram Bot API](https://core.telegram.org/bots/api)
- [Dialogflow Intents & Entities Guide](https://cloud.google.com/dialogflow/docs/basics)

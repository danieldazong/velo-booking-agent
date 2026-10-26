# Velo: AI Conversational Booking Engine

![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)
![Status: Production](https://img.shields.io/badge/Status-Production-success.svg)

Velo is an autonomous scheduling architecture that replaces rigid booking forms with a fluid, intelligent conversational agent[cite: 124]. It actively negotiates meeting times, collects required contact data, and seamlessly generates Google Meet calendar invitations without human intervention[cite: 124].



## 🔗 Live Demo
- **Live Website:** (https://nouvrix-booking.netlify.app/)
- **Deployment Platform:** n8n (Backend) / Netlify (Frontend)



## 📌 Project Overview
This repository contains the backend n8n workflow and the custom HTML/JS frontend code for the Velo scheduling agent. The system completely manages the friction of scheduling, ensuring no incomplete or invalid appointments ever reach your calendar[cite: 124].

### Key Highlights
- **Conversational Gatekeeper:** Evaluates user requests against a strict internal checklist (Topic, Time, Duration, and Email) before triggering the calendar tool[cite: 124].
- **Custom Web Interface:** Replaces standard widgets with a premium, branded chat interface featuring dark-mode aesthetics, custom gradients, and interactive pill-buttons[cite: 124].
- **Smart Formatting & Parsing:** Automatically converts raw Google Meet URLs returned by the AI into clickable hyperlinks in the chat UI[cite: 124].
- **Secure Memory Isolation:** Generates unique session IDs on page load to ensure conversation memory remains private and separated between concurrent visitors[cite: 81, 124].



## 🛠 Tech Stack

| Category | Technology |
| :--- | :--- |
| **Workflow Engine** | n8n (Agentic Architecture) |
| **AI / LLM** | OpenAI API (gpt-4o-mini) |
| **Database / CRM** | Google Calendar API |
| **Frontend UI** | HTML / CSS / Vanilla JS |
| **Version Control** | Git & GitHub |



## 📁 Repository Structure

├── assets/                  # Static assets (logos, custom SVG icons)
├── docs/                    # Architecture diagrams and operational guides
├── sample-data/             # Synthetic testing payloads
├── .env.example             # Template for API keys & OAuth setup
├── .gitignore               # Specifies local files Git should ignore
├── README.md                # Project documentation and setup guidelines
├── index.html               # Custom frontend chat interface and web app
└── workflow.json            # The core Agentic AI scheduling workflow



## 🚀 Getting Started

Follow these instructions to run a copy of the project locally for development or testing purposes.

### Prerequisites

- A modern web browser (Chrome, Edge, Firefox, Safari)
- [Git](https://git-scm.com/) installed on your local machine
- An active n8n instance (Local desktop app or Cloud)
- A Google Cloud Console project with Calendar API enabled

### Installation & Local Setup

1. **Clone the repository:**

git clone https://github.com/danieldazong/velo-booking-agent.git
cd velo-booking-agent


2. **Configure Environment Variables:**

Duplicate the `.env.example` file, rename it to `.env`, and populate your OpenAI and Google Calendar OAuth credentials.


3. **Import Workflows into n8n:**

Open your n8n workspace, navigate to the workflows dashboard, and select **Import from File**. Upload `workflow.json` from the root directory. Ensure the workflow is toggled to **Active** to receive webhook payloads.


4. **Run the local development server:**

Open `index.html` in your text editor and replace the `N8N_PRODUCTION_WEBHOOK` variable with your live n8n Chat Trigger URL. Launch `index.html` in your browser to test the conversational interface locally.



## 📬 Contact & Connect

- **Developer:** Daniel Dazong
- **LinkedIn:** https://www.linkedin.com/in/danieldazong
- **GitHub:** https://github.com/danieldazong
- **Email:** danieldazong08@gmail.com

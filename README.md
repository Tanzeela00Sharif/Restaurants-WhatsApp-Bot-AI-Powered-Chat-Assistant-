# Restaurants-WhatsApp-Bot-AI-Powered-Chat-Assistant-
📖 Overview

This project demonstrates an AI-driven WhatsApp chatbot built using n8n, OpenAI, Supabase, and Postgres.
The chatbot automates restaurant interactions such as responding to customer queries, handling bookings, and maintaining conversational memory.

It combines:

WhatsApp Chatbot Automation (via n8n Trigger)

AI-Powered Responses using OpenAI

Memory Management using Postgres

Knowledge Retrieval (RAG) using Supabase Vector Store & Embeddings

🧩 Workflow Components
🟢 WhatsApp Bot Trigger

Captures incoming WhatsApp messages via n8n webhook and initiates the workflow.

🤖 AI Agent

Processes user messages and generates contextual replies using OpenAI Chat Model.
It maintains conversational context through Postgres-based memory.

🧠 Supabase Vector Store (RAG Pipeline)

Implements Retrieval-Augmented Generation (RAG).
It downloads reference documents, creates embeddings using OpenAI Embeddings, and stores them in Supabase for semantic search and knowledge retrieval.

📤 Send Message Node

Sends AI-generated responses back to WhatsApp users.

⚙️ Workflow Overview (Architecture)
WhatsApp Trigger → AI Agent → Send Message
                   ↘ Memory (Postgres)
                   ↘ Tool (Supabase Vector Store)
                     ↘ OpenAI Embeddings
                     ↘ RAG Document Loader

🛠️ Setup Instructions

Clone this Repository

git clone https://github.com/TanzeelaSharif/Restaurants-WhatsApp-Bot.git
cd Restaurants-WhatsApp-Bot


Open n8n

Import the provided n8n workflow (.json file if exported).

Configure your environment variables for:

WhatsApp Cloud API credentials

OpenAI API key

Supabase project URL & API key

Postgres connection (if used for chat memory)

Run the Workflow

Start n8n (either locally or hosted).

Send a WhatsApp message like “Hi” to trigger the workflow.

The bot will respond automatically and handle conversation intelligently.

🎥 Add Demo Video to GitHub
Option 1: Upload to GitHub Repository

You can directly add your demo video file (demo.mp4) to the repository:

Place the video in your project root folder.

Commit and push:

git add demo.mp4
git commit -m "Added demo video"
git push origin main


Then link it in your README:

### 🎬 Demo Video

[🎥 Watch the demo]("C:\Users\USER\Videos\Screen Recordings\C.mp4")



Option 2: Add via YouTube

If your video is large or hosted on YouTube:

Upload it to YouTube (set to Public or Unlisted).

Add the video preview in README:

### 🎬 Demo Video
[![Watch the demo](https://img.youtube.com/vi/YOUR_VIDEO_ID/0.jpg)](https://www.youtube.com/watch?v=YOUR_VIDEO_ID)

🧩 Technologies Used

n8n – Workflow automation

OpenAI GPT Model – Chat and embeddings

Supabase – Vector storage for RAG

Postgres – Chat memory

WhatsApp Cloud API – Messaging platform

🌐 Author

Tanzeela Sharif
📍 MS Data Science | Data Analyst | AI Enthusiast
🔗 GitHub Profile

📧 tanzeelasharif@gmail.com
 (optional if you want to add it)

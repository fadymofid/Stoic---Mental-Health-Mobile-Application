# Stoic

Stoic is a cross-platform mobile application designed to provide accessible, affordable, and stigma-free mental health support. Leveraging AI-driven emotion detection, personalized coping strategies, and community engagement, Stoic acts as a virtual life coach to help users manage stress, anxiety, and depression.

## Features

* **Emotion Analysis via Chatbot**

  * Real-time sentiment detection (stress, anxiety, depression, suicidal ideation) using DeepSeek-R1.
  * Emotion logging and trend visualization over time.
* **Mood Tracking & Insights**

  * Weekly check-ins and daily mood logging.
  * Interactive charts to visualize emotional progress.
* **Personalized Coping Strategies**

  * Contextual recommendations: mindfulness, breathing exercises, self-care routines.
  * Guided journaling prompts.
* **AI Chat Functionality**

  * Multi-turn dialogues with context persistence.
  * Session management and history with delete options.
* **Onboarding & Decision Tree Assessment**

  * Initial questionnaire to tailor content and resources.
  * Skip option with default "normal" status.
* **Community & Rooms**

  * Create, join, and manage public/private chat rooms.
  * Post, comment, like, react, and moderate content.
* **Real-Time Notifications**

  * Push and in-app alerts for check-ins, messages, and community activity.
  * Read status and inbox management via WebSockets.
* **Localization**

  * Full support for English and Arabic (RTL layout).
  * Persistent language preference per user.
* **Security & Validation**

  * Role-based access control (Admin vs. Regular User).
  * Input validation, profanity filtering, and error handling.

## Tech Stack

* **Frontend**: React Native
* **Backend**: Spring Boot, Java
* **Database**: MySQL
* **AI & NLP**: DeepSeek-R1 sentiment analysis model
* **Deployment**: Docker, Docker Compose, OpenShift
* **Testing**: JUnit, Mockito, React Testing Library

## Prerequisites

* Node.js (>=14)
* npm or yarn
* Java 11+
* Docker & Docker Compose
* OpenShift CLI (for production deployment)

## Installation & Running Locally

1. **Clone the repository**

   ```bash
   git clone https://github.com/your-org/stoic.git
   cd stoic
   ```

2. **Backend Setup**

   * Configure `application.properties` with your MySQL credentials.
   * Build and run with Docker Compose:

     ```bash
     docker-compose up --build
     ```
   * The Spring Boot API will be available at `http://localhost:8080`.

3. **Mobile App Setup**

   ```bash
   cd mobile
   npm install
   npm run start
   ```

   * Open the Expo client on your device or simulator.

4. **Environment Variables**

   * Create a `.env` file in the `mobile` folder with API URL and DeepSeek API key:

     ```ini
     API_URL=http://localhost:8080/api
     DEEPSEEK_KEY=your_deepseek_key
     ```

## Usage

1. **Onboarding**: Complete the initial assessment or skip to start using Stoic.
2. **Chatbot**: Send messages to receive AI-driven support and coping strategies.
3. **Check-Ins**: Answer weekly questionnaires to track your mood.
4. **Community**: Join rooms, share posts, and engage with peers.
5. **Settings**: Change language, update profile, and manage notifications.






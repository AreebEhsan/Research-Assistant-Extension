# 🔍 Research Assistant - AI-Powered Content Summarizer Tool

**Research Assistant** is a dual-module productivity tool that combines a **Spring Boot backend** with a **Chrome Extension frontend** to provide intelligent summarization and topic suggestions using the Gemini AI API.

> 📚 Just highlight text, click summarize, and get instant insights. Ideal for students, researchers, and writers!

---

## Features

### Gemini AI Integration (via Spring Boot Backend)
- Summarizes large chunks of text into concise, readable summaries.
- Suggests related research topics and further reading, formatted with bullet points.
- Uses Google's Gemini AI API via `WebClient` (non-blocking HTTP client).
- Handles JSON parsing via Jackson and structured response handling via Lombok.

### 🌐 Chrome Extension (Frontend)
- Clean, minimal UI with:
  - **Summarize** button
  - **Note-taking area** with save functionality
- Injects into webpages for seamless integration with articles, research papers, blogs, etc.

---


---

## ⚙️ Backend Setup (Spring Boot)

### ✅ Prerequisites:
- Java 21+
- Maven 3.8+
- A valid Gemini API key

### 📦 Build & Run

```bash
# Navigate to backend directory
cd research-assistant-backend

# Build the project
./mvnw clean install

# Run the Spring Boot application
./mvnw spring-boot:run

## 🌍 Chrome Extension Setup

### Load Locally

1. Go to `chrome://extensions/`
2. Enable **Developer mode**
3. Click **Load unpacked**
4. Select the `research-assistant-extension` directory

You’ll see a panel with:

- 🧠 **Summarize** button (which calls the Spring Boot API)
- 📝 **Note section** to manually store findings

---



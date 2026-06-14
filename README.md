# AI Assistant Platform - Intelligent Chat Application

## 🔗 Live Demo
Access the live application here: **[https://ai-assistant-platform-seven.vercel.app](https://ai-assistant-platform-seven.vercel.app)**

AI Assistant Platform is a modern, feature-rich conversational interface built using Next.js and the Vercel AI SDK. It supports real-time streaming, multi-session interactive chats, historical query persistence, and multiple LLM models.

## 🚀 Key Features

* **Real-time Streaming:** Extremely fast response streaming from LLM APIs.
* **Interactive Chat History:** Seamless session management, listing, and persistence for multiple parallel conversation contexts.
* **Auth & Profiles:** Simple and secure credential-based login and session handling via Auth.js.
* **Modern Design:** Built with React 19, Tailwind CSS, and Radix UI components for a premium dark-themed experience.
* **Data Storage:** High-performance data persistence with Drizzle ORM and Neon Serverless Postgres, and image/file upload handling via Vercel Blob.

## 🛠️ Tech Stack

* **Front-End & Framework:** Next.js (App Router), React 19, Tailwind CSS, Radix UI (shadcn/ui), Framer Motion
* **AI Integration:** Vercel AI SDK, OpenAI API, Anthropic Claude, Gemini, etc.
* **Database & Auth:** Neon Postgres, Drizzle ORM, Auth.js (NextAuth)

---

## 💻 Local Setup & Run

Follow these instructions to run the AI Assistant Platform on your local machine.

### 1. Clone & Install Dependencies
```bash
git clone https://github.com/NI3HIL/ai-assistant-platform.git
cd ai-assistant-platform
npm install
```

### 2. Configure Environment Variables
Copy `.env.example` to `.env.local` and configure your API keys:
```bash
cp .env.example .env.local
```
Update the `.env.local` file with:
* `OPENAI_API_KEY` (or other LLM provider keys)
* `POSTGRES_URL` (PostgreSQL connection string)
* `AUTH_SECRET` (Run `npx auth secret` to generate)

### 3. Migrate Database
Generate and apply database migrations to setup the schema:
```bash
npm run db:push
```

### 4. Start Development Server
Run the local dev server:
```bash
npm run dev
```
Open `http://localhost:3000` in your browser to test the application.

---

## 📄 License
MIT License

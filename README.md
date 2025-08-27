## **Backend README (`mood-ai-backend/README.md`)**

```markdown
# Mood AI Backend

A NestJS-based backend for mood tracking with real-time updates and AI insights.

---

## Features
- REST API for submitting and retrieving moods
- WebSocket gateway for real-time updates
- SQLite database for quick setup
- Gemini API integration for AI mood suggestions

---

## Tech Stack
- **NestJS** - Backend framework
- **TypeORM** - ORM for database
- **SQLite** - Database
- **Socket.IO** - Real-time events
- **Axios** - API requests to Gemini

---

## Getting Started

### 1. Clone Repository
```bash
git clone <repo-url>
cd mood-ai-backend
````

### 2. Install Dependencies

```bash
npm install
```

### 3. Configure Environment Variables

Create `.env` file:

```
PORT=3000
GEMINI_API_KEY=your-gemini-api-key
```

### 4. Run Development Server

```bash
npm run start:dev
```

---

## Project Structure

```
src/
├── mood/                 # Mood module (controller, service, entity)
├── app.module.ts         # Main app module
└── main.ts               # Entry point
```

---

## API Endpoints

### POST /mood

Submit mood data.

### GET /mood

Fetch all mood data.

---

## WebSocket Events

* **moodUpdated** → Broadcasts whenever a new mood is submitted.

---

## Build for Production

```bash
npm run build
npm run start:prod
```
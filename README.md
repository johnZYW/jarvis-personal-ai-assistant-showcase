# Jarvis Personal AI Assistant Showcase

Public showcase repository for the Jarvis iOS personal AI assistant prototype.

> Core implementation is currently closed-source. This repository contains only the public project package: overview, architecture notes, demo video, and safety/privacy boundary. The latest iOS app source code, production backend implementation, local databases, credentials, logs, and user data are intentionally excluded.

## Project overview

Jarvis is an iOS personal AI assistant prototype that turns natural-language requests into safe, structured, and verifiable personal workflow actions. It is designed as more than a chatbot: it coordinates calendar planning, task management, document/meeting preparation, weather-aware planning, local-service recommendations, travel comparison, and cost tracking.

The app uses a React Native / Expo iOS frontend, a FastAPI backend, SQLite sandbox storage, and an LLM orchestration layer. The backend is organized around bounded contexts such as calendar, tasks, document memory, travel, local services, weather, and money/cost tracking. User-data mutations are confirmation-first: Jarvis prepares a review card before executing actions such as calendar edits, itinerary saves, compound schedule drafts, or cost creation.

## Demo video

- [Jarvis real-user demo video](./jarvis_real_user_demo.mp4)

The demo presents Jarvis as an AI full-stack assistant: the app interprets a user request, routes it through assistant capabilities, exposes confirmation/review surfaces, and updates application state around calendar, travel, local-service planning, files, and cost tracking.

## What the demo shows

- Morning brief: weather, yesterday recap, today schedule, and next useful action.
- Calendar operations: schedule lookup, meeting reschedule, conflict warning, confirmation-first mutation, and calendar verification.
- File and meeting prep: mock PDF, DOCX, and spreadsheet discovery with in-app preview.
- Local-service planning: restaurant recommendations with rating, distance, phone number, and dinner windows.
- Travel comparison: flight and hotel options ranked by price, duration, and trade-off score.
- Money beside Calendar: confirmed dinner and itinerary drafts save planned costs into a compact cost view.
- Safety surface: cards for review, confirmation, choices, completed actions, and structured objects.

## Technical scope

- **Frontend**: React Native / Expo iOS interface.
- **Backend**: FastAPI service layer.
- **Data**: SQLite sandbox stores for demo-safe state management.
- **AI layer**: LLM orchestration, intent parsing, action frame generation, clarification, and response synthesis.
- **Tool/capability layer**: calendar, tasks, local services, document memory, travel, weather, attachments, and money/cost tracking.
- **Safety layer**: confirmation-first mutation for calendar changes, itinerary saves, compound schedule drafts, and cost creation.
- **QA layer**: simulator-based golden journey, scenario tests, smoke tests, and UX replay review.

## Architecture

See [`architecture/ARCHITECTURE.md`](./architecture/ARCHITECTURE.md).

## Public / private boundary

Public in this repository:

- Project overview
- Architecture summary
- Demo video
- Security and privacy note

Private for now:

- Latest iOS app source code
- Production backend implementation
- User data, credentials, logs, local databases, and live adapters

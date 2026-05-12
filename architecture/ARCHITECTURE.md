# Jarvis Architecture Summary

Jarvis is presented as an AI full-stack personal assistant prototype.

## Product layers

1. **iOS frontend**: React Native / Expo mobile interface for chat, calendar, tasks, settings, cards, and review surfaces.
2. **Backend service**: FastAPI service layer for assistant orchestration and bounded-context modules.
3. **LLM orchestration**: Natural-language request parsing, action frame generation, clarification, and response synthesis.
4. **Tool / capability layer**: Calendar, tasks, local services, document memory, travel, weather, attachments, and money/cost tracking.
5. **Data layer**: SQLite-backed sandbox stores for demo-safe state management.
6. **Safety layer**: Confirmation-first mutation for calendar changes, itinerary saves, compound schedule drafts, and cost creation.
7. **QA layer**: Simulator-based golden journey, scenario tests, smoke tests, and UX replay review.

## Closed-source note

The latest Jarvis app implementation is not fully open-sourced in this showcase repository. This repository is intended for competition review and portfolio demonstration, containing public documentation, demo materials, and non-sensitive engineering notes.

## AI full-stack challenge narrative

The project is framed as a demonstration of a “super individual”: a developer using AI coding tools to move from requirements and product design to backend architecture, mobile interface, LLM tool orchestration, safety mechanism, regression testing, documentation, and demo packaging.

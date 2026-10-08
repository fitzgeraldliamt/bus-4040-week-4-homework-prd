# PRD: CBE Speaker & Event Schedule Application

## 1. Problem Statement

The event planning team for CBE's executive education programs manages past event data that lives in manually created files of varying formats, authored by different people over time. There is no centralized, searchable repository for speaker information, and no standardized workflow for building or editing event schedules.

## 2. Goals

- **Data access:** Enable event planners to search, filter, and input event and speaker data through a single, easy-to-use interface.
- **Data migration:** Populate the application with all historical event and speaker data (2016–2026) from the existing legacy files, so no information is lost in the transition.
- **Schedule building:** Provide a workspace where planners can quickly assemble, reorder, and save event schedules without re-typing speaker details.

## 3. Constraints

| # | Constraint | Detail |
|---|-----------|--------|
| 1 | **Deadline** | All deliverables are due by the end of the semester (mid-December 2026). |
| 2 | **Data scope** | Historical data from 2016 through 2026 must be migrated into the application before the deadline. This is not optional or deferred. |
| 3 | **Budget / resources** | No external budget is specified; the project is scoped to available course resources and student effort. *(Adjust if your project has budget or additional resources.)* |
| 4 | **Technical / platform** | The application will be a standard web application accessible via desktop or laptop browsers. No native mobile app is required. |
| 5 | **User scope** | The tool is for CBE's internal event planning team only. No public-facing or client-facing interface is in scope. |
| 6 | **Compatibility** | The data import process must handle the mixed formats found in the legacy files (spreadsheets, slides, PDFs, or other manually created documents). |

> *Note: Constraints 3–5 are inferred from the client scenario and common class-project assumptions. Flag or revise if they don't match your actual situation.*

## 4. Target Users / Personas

Event planners and administrators.

## 5. User Stories

- **As a** planner **I want to** search and recall speaker information (names, titles, past appearances, contacts) **so that** I can re-invite speakers from previous years' programs.
- **As a** planner **I want to** review details from past events (schedules, session formats, venues) **so that** I can use them as a template when building this year's event.
- **As a** planner **I want to** build and edit a schedule for the upcoming event **so that** I can plan the event itself — assigning speakers to sessions, setting times, and saving the final agenda.

## 6. Functional Requirements

**FR-1: Speaker Management**
- The system shall allow users to create, view, update, and archive speaker records.
- Speaker records shall include at minimum: name, affiliation/title, email, phone, past event appearances, and notes.
- The system shall support searching and filtering speakers by name, affiliation, event, and year.

**FR-2: Event Management**
- The system shall allow users to create, view, update, and archive event records.
- Event records shall include at minimum: program name (e.g., Energy Executive Course), event name, date(s), location, and status.
- The system shall support searching and filtering events by program, year, and date range.

**FR-3: Schedule Building**
- The system shall allow users to build an event schedule by assigning speakers to sessions.
- Users shall be able to define sessions with a title, start time, end time, and associated speaker(s).
- Users shall be able to reorder, add, remove, and edit sessions within a schedule.
- Users shall be able to save multiple versions of a schedule (draft → final).

**FR-4: Data Import / Migration**
- The system shall import all historical event and speaker data (2016–2026) from the existing legacy files.
- The import process shall handle the mixed formats present in the legacy files (e.g., spreadsheets, slides, PDFs).
- After import, the data shall be viewable and searchable within the application.

**FR-5: Output / Export**
- The system shall allow users to export a finalized schedule in a shareable format (e.g., PDF or printable view).

## 7. Out of Scope

The following items are explicitly excluded from this project's scope:

- **Real-time collaboration** — multiple users editing the same schedule simultaneously with live sync, merge resolution, or presence indicators.
- **Public-facing features** — any web portal, registration, or information page accessible to event attendees, sponsors, or the general public.
- **Notification and workflow automation** — automated email reminders to speakers, approval chains, or status change alerts.
- **Mobile applications** — native iOS/Android apps or mobile-optimized experiences. The application will be accessible via standard desktop web browsers.
- **Budget, finance, or contract management** — tracking speaker fees, sponsorships, or program budgets.
- **Third-party integrations** — connections to external calendar systems (Google Calendar, Outlook), CRM platforms, or registration tools.
- **Analytics and reporting** — dashboards, usage metrics, or event performance analytics beyond the basic search and retrieval of historical data.
- **Multilingual support** — the application will be in English only.

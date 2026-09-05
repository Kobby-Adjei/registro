# Registro

Registro is an event discovery and management platform built to make finding, creating, and managing events simple. Organizers can publish events, manage registrations, and track attendance from one place, while attendees can discover events, register, and keep track of what’s coming up.

## MVP

The first release focuses on the complete event lifecycle:

1. Organizer creates an event.
2. Event is published and becomes discoverable.
3. Attendee views event details.
4. Attendee registers.
5. Organizer views registrations.
6. Attendee sees the event under My Events.

## Core Features

- Authentication and user profiles
- Event creation and editing
- Event discovery and filtering
- Event detail pages
- Event registration and cancellation
- My Events
- Organizer dashboard
- Basic registration statistics

## Repository Structure

```text
registro/
├── frontend/              # Frontend application
├── backend/               # Backend/API application
├── docs/
│   ├── product/           # Product requirements and specifications
│   ├── architecture/      # Architecture diagrams and technical decisions
│   └── meeting-notes/     # Team meeting notes and decisions
├── .github/
│   ├── ISSUE_TEMPLATE/    # Issue templates
│   └── PULL_REQUEST_TEMPLATE.md
├── CONTRIBUTING.md
└── README.md
```

## Status

**Phase:** Product definition and technical setup

The team is currently finalizing product scope, technical stack, and application architecture before implementation begins.

## Team Workflow

- Keep `main` stable.
- Build each task on its own branch.
- Open a pull request before merging into `main`.
- Keep pull requests focused on one feature or fix.
- Use GitHub Issues to track features, bugs, and technical work.

Recommended branch names:

- `feature/event-creation`
- `feature/authentication`
- `feature/event-discovery`
- `fix/registration-validation`
- `docs/database-design`

## Roadmap

1. Finalize product scope.
2. Choose the technical stack.
3. Define the data model.
4. Define the application architecture.
5. Build authentication.
6. Build event creation and management.
7. Build event discovery.
8. Build registration workflows.
9. Build the organizer dashboard.
10. Test and polish the end-to-end experience.

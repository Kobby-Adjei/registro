# Registro

Registro is a semester software-engineering project for COSC 482W. The product is an event discovery and management platform where organizers can create and manage events, and attendees can discover, register for, and track events.

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

## Development Status

**Phase:** Product definition / project setup

The technical stack and detailed architecture will be selected by the team before implementation begins.

## Team Workflow

- `main` should remain stable.
- Each task should be developed on its own branch.
- Open a pull request before merging work into `main`.
- Keep pull requests focused on one feature or fix.
- Use GitHub Issues to track features, bugs, and technical tasks.

Recommended branch names:

- `feature/event-creation`
- `feature/authentication`
- `feature/event-discovery`
- `fix/registration-validation`
- `docs/database-design`

## Initial Development Order

1. Confirm product scope.
2. Choose technical stack.
3. Define database/data model.
4. Define application architecture.
5. Build authentication.
6. Build event creation and management.
7. Build event discovery.
8. Build registration workflow.
9. Build organizer dashboard.
10. Test and polish the complete user flow.

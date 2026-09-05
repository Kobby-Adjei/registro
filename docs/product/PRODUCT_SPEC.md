# Registro — Product Specification v1

## Product Overview

Registro is an event discovery and management platform that allows people to create events, discover events that interest them, register to attend, and manage their participation from one place.

Organizers will be able to publish events, manage registrations, communicate important event information, and view basic attendance data. Attendees will be able to browse upcoming events, view event details, register, and keep track of events they plan to attend.

The initial version will focus on providing a simple and reliable event-management experience rather than attempting to reproduce every feature available in larger event platforms.

## Problem

Event information is often spread across social media posts, flyers, group chats, emails, and separate registration forms. This creates several problems:

- People miss events they would have been interested in.
- Organizers have to use multiple tools to promote and manage an event.
- Registration information can become difficult to manage.
- Attendees may forget events after registering.
- Organizers have limited visibility into registration and attendance.

Registro will provide a central location for event discovery, registration, and management.

## Target Users

### Attendees

Attendees should be able to:

- Discover upcoming events.
- Search or filter events.
- View event information.
- Register for an event.
- View their registered events.
- Cancel a registration if necessary.

### Organizers

Organizers should be able to:

- Create an event.
- Edit event information.
- Publish or cancel an event.
- View registered attendees.
- Track registrations.
- Manage basic event information from a dashboard.

## Product Goals

The first version should allow a user to complete the entire event lifecycle:

**Organizer creates event → event becomes discoverable → attendee finds event → attendee registers → organizer sees registration → attendee attends event.**

The product should also:

- Make event creation simple.
- Make relevant event information easy to find.
- Reduce the number of separate tools organizers need.
- Give organizers basic information about their events.
- Provide a clean and intuitive user experience.

## MVP Features

### Authentication

Users can:

- Create an account.
- Sign in.
- Sign out.
- Maintain a basic profile.

A user may act as both an attendee and an organizer.

### Event Creation

Organizers can create an event containing:

- Event title
- Description
- Cover image
- Date
- Start time
- End time
- Location
- Event category
- Organizer information
- Registration capacity, if applicable

### Event Management

Organizers can:

- View events they created.
- Edit event information.
- Publish an event.
- Cancel an event.
- View the number of registrations.
- View registered attendees.

### Event Discovery

Users can browse upcoming events. Each event card should display basic information such as:

- Event name
- Date
- Time
- Location
- Image
- Category

Users should also be able to search or filter events by basic criteria such as category or date.

### Event Details

Selecting an event opens an event page containing:

- Event title
- Description
- Date and time
- Location
- Organizer
- Event image
- Registration information
- Register button

### Event Registration

Users can register for an event. The system should:

1. Confirm that the user is logged in.
2. Confirm that registration is available.
3. Create the registration.
4. Show confirmation to the attendee.
5. Add the attendee to the organizer's registration list.

Users should not be able to register for the same event multiple times.

### My Events

Attendees will have a page showing:

- Upcoming events
- Past events

The user should also be able to cancel an upcoming registration when registration rules allow it.

### Organizer Dashboard

Organizers will have a dashboard showing their events. For each event, the dashboard can display:

- Event status
- Date
- Number of registrations
- Capacity
- Attendee list

Basic summary statistics may include:

- Total events created
- Total registrations
- Registrations per event

## Core User Flows

### Organizer Flow

Sign in → Create Event → Enter event information → Publish Event → Event appears in discovery → Users register → Organizer views registrations

### Attendee Flow

Sign in → Browse Events → Select Event → View Details → Register → Receive confirmation → Event appears under My Events

## Initial Data Model

### User

- user_id
- name
- email
- profile_image
- created_at

### Event

- event_id
- organizer_id
- title
- description
- image
- category
- location
- start_datetime
- end_datetime
- capacity
- status
- created_at

### Registration

- registration_id
- event_id
- user_id
- registration_status
- registered_at

## Event Statuses

- Draft
- Published
- Cancelled
- Completed

Only published events should appear in public event discovery.

## Non-Goals for the Initial Version

The first release will not require:

- Full payment processing
- Ticket resale
- Complex recommendation algorithms
- Livestreaming
- Advanced social networking
- Large-scale marketing automation
- Complex organization permissions
- Native iOS or Android applications

## Possible Future Features

- Personalized event recommendations
- QR-code event check-in
- Event reminders
- Waitlists
- Saved/favorite events
- Organizer analytics
- Calendar integration
- Event sharing
- Event comments or discussion
- Organization profiles
- Email notifications
- AI-assisted event descriptions
- Location-based event discovery

## Success Criteria

The MVP is successful if a new user can:

1. Create an account.
2. Discover an event.
3. View its details.
4. Register for it.
5. See it in their upcoming events.

An organizer must also be able to:

1. Create an event.
2. Publish it.
3. Receive registrations.
4. See who registered.
5. Edit or manage the event.

## Development Priority

### Phase 1 — Foundation

- Authentication
- Database structure
- User profiles
- Basic application navigation

### Phase 2 — Events

- Create event
- Edit event
- Event details
- Event discovery

### Phase 3 — Registration

- Register for event
- Cancel registration
- My Events
- Organizer attendee list

### Phase 4 — Management

- Organizer dashboard
- Event status management
- Basic statistics

### Phase 5 — Polish

- Testing
- Error handling
- Responsive design
- Performance improvements
- User experience improvements

## Product Principle

The team should prioritize completing the core event lifecycle before adding advanced features. A smaller product where event creation, discovery, registration, and management work reliably is more valuable than a large feature set with incomplete workflows.

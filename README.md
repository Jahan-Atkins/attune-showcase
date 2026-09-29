# Attune (Showcase)

A full-stack gig-work marketplace that connects yoga and sound bath instructors with customers.

> This is a showcase repo. The source code is private. Code walkthroughs are available on request.

**Demo video:** [ADD UNLISTED YOUTUBE LINK]
**Contact:** Jahan.atkins815@gmail.com | linkedin.com/in/jahan-atkins-39002b419

## What it does
- Instructors manage clients, sessions, and availability.
- Customers browse and book sessions.
- An auto-matching flow links customers to instructors.
- Each user only sees their own data.

## Tech stack
| Layer | Tools |
|---|---|
| Backend | Python, FastAPI |
| Database | SQLAlchemy, SQLite, Alembic migrations |
| Auth | JWT-based authentication |
| Testing | pytest (41 passing tests) |
| Frontend | Separate instructor and customer frontends |

## Highlights
- **Access control:** Data is scoped per user, and tests verify one user cannot read another user's data.
- **Testing:** 41 automated tests cover authentication, CRUD operations, and data isolation.
- **Matching:** A booking and matching flow connects the two sides of the marketplace.
- **Migrations:** Schema changes are managed with Alembic.

## Architecture
```
Instructor frontend --\
                       >-- FastAPI --> SQLAlchemy --> SQLite
Customer frontend  ---/        |
                          JWT auth
```

## Screenshots
Add images to the `screenshots/` folder and link them here.

## What I learned
- Designing an API with authentication and per-user data isolation
- Writing tests that catch access-control bugs
- Managing database migrations
- Building two separate frontends against one backend

## Roadmap
Availability blocks, distance-based matching, and overlap detection for scheduling.

# Next.js Architecture Skill

This project uses Next.js with the App Router.

## Core Principles

Prefer server components whenever possible.

Client components should only be used when:
- user interaction requires state
- browser APIs are needed
- a third-party library requires client rendering

Avoid unnecessary client-side logic.

---

## Routing Structure

Use the App Router.

Example structure:

/app
  /dashboard
    page.tsx
  /projects
    page.tsx
  /projects/[id]
    page.tsx

Do not create deeply nested routes without a clear reason.

---

## Data Fetching

Prefer server-side data fetching.

Example:

const projects = await getProjects()

Avoid unnecessary client fetching.

---

## API Routes

Use API routes for backend logic.

/app/api/projects/route.ts

API routes must:
- validate inputs
- handle errors
- return structured responses

---

## File Organization

/components
  /ui
  /features

/ui = reusable components  
/features = domain-specific components

---

## Performance

Avoid large client components.

Split large UI sections into smaller components.

Lazy load heavy UI elements.
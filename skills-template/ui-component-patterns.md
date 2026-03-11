# UI Component Patterns Skill

The UI uses Tailwind CSS.

## Styling

Use Tailwind utility classes.

Avoid large CSS files.

---

## Component Structure

Reusable UI components:

/components/ui

Feature-specific components:

/components/features

---

## Component Design Rules

Components should:

- have one responsibility
- remain under ~200 lines when possible
- avoid complex internal logic

---

## Layout

Use consistent layout containers.

Example:

max-w-6xl mx-auto px-6

---

## Interaction Feedback

Always provide:

- loading states
- error messages
- success confirmations
# TypeScript Standards Skill

All code must be written in TypeScript.

## Type Safety

Avoid the "any" type.

Define interfaces for structured data.

Example:

interface Project {
  id: string
  title: string
  created_at: string
}

---

## Data Models

Each database entity should have a corresponding interface.

Store shared types in:

/types

Example:

/types/project.ts

---

## Function Design

Functions must include explicit types.

Example:

async function createProject(title: string): Promise<Project>

---

## Error Handling

Always check for errors returned from APIs.

Never silently ignore errors.

---

## Readability

Prefer simple, readable code.

Avoid complex generics unless absolutely necessary.
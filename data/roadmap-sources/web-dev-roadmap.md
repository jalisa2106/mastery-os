# Next.js + NestJS — 12 Week Manual Coding Roadmap

**Goal:** Go from "reads AI-generated code well" to "writes it from scratch without AI."
**Time:** 30-45 min/day. **Rule:** No AI, no copy-paste, no docs-open-first during practice. Try from blank file, then check yourself.

---

## Week 1 — JS Fundamentals You've Been Outsourcing

- **Day 1:** Array methods — write `map` from scratch (no built-ins allowed, then compare to real one)
- **Day 2:** Array methods — write `filter` and `reduce` from scratch on a sample array and compare
- **Day 3:** Destructuring + spread/rest — rewrite 5 functions using destructured params
- **Day 4:** Promises — fetch data using callbacks and `.then()` promises
- **Day 5:** async/await — rewrite fetch using async/await with try/catch error handling
- **Day 6:** Review — redo Day 1 and Day 4 from memory, no peeking
- **Day 7:** Rest / light review of anything shaky

## Week 2 — Closures, context, and JS Review

- **Day 8:** Closures — write a counter factory function and explain out loud why it works
- **Day 9:** `this` context, arrow functions vs regular functions — write 3 examples showing the difference
- **Day 10:** `this` context — practice binding and lexical scope exercises in handler functions
- **Day 11:** Review — redo Day 8 and Day 9 from memory
- **Day 12:** JS fundamentals synthesis — build a mini fetch cache using closures and promises
- **Day 13:** Checkpoint — JS fundamentals final self-assessment
- **Day 14:** Rest / light review of JS concepts

## Week 3 — React Core — State & Effects

- **Day 15:** `useState` — build a counter + a toggle component from a blank file
- **Day 16:** `useState` — practice state updates with complex objects and arrays (no helper libraries)
- **Day 17:** `useEffect` — build a component that fetches data on mount, handle loading state
- **Day 18:** `useEffect` — handle error states and component cleanups in effects
- **Day 19:** Props vs state — build a parent component passing data + a callback to a child
- **Day 20:** Review — rebuild Day 15 and Day 17 from memory
- **Day 21:** Rest / light review of React state and effects

## Week 4 — React Core — Lists, Forms, & Composition

- **Day 22:** Lists and keys — build a todo list (add/remove items) from scratch
- **Day 23:** Forms — build a controlled form with 3 inputs and validation on submit
- **Day 24:** Component composition — refactor todo list into 3 smaller components
- **Day 25:** Component composition — practice composition by passing components as props
- **Day 26:** Rebuild the todo list entirely from memory, timed — no reference
- **Day 27:** Redo memory build — optimize component render cycles and state layout
- **Day 28:** Rest / light review of forms and component layout

## Week 5 — Next.js Fundamentals (App Router)

- **Day 29:** File-based routing — create `app/about/page.tsx`, `app/blog/page.tsx` manually
- **Day 30:** Dynamic routes — build `app/blog/[slug]/page.tsx`, log the param
- **Day 31:** Layouts — create a shared `layout.tsx` with a nav bar across routes
- **Day 32:** Server vs Client Components — write one of each, explain why each needs (or doesn't need) `"use client"`
- **Day 33:** Data fetching in Server Components — fetch a public API directly in a page component
- **Day 34:** Loading and error states — add `loading.tsx` and `error.tsx` to a route
- **Day 35:** Rest / light review of Next.js routing

## Week 6 — Next.js Route Handlers & Data

- **Day 36:** Route handlers — create `app/api/notes/route.ts` with a GET handler returning mock data
- **Day 37:** POST handler — accept a body, validate it, return a response
- **Day 38:** Dynamic API routes — create GET and DELETE handlers for `app/api/notes/[id]/route.ts`
- **Day 39:** Connect a page to your own API route (fetch from `app/api/notes` in a Server Component)
- **Day 40:** Client-side interactivity — add a delete button that calls your DELETE route
- **Day 41:** Environment variables + `.env.local` — use one in a route handler
- **Day 42:** Rest / light review of Next.js APIs

## Week 7 — Next.js Review & NestJS Core

- **Day 43:** Notes App — build end-to-end note app (GET list, POST add, DELETE)
- **Day 44:** Rebuild the Notes app from memory, timed — no notes open
- **Day 45:** Install Nest CLI, generate a project, understand the folder structure by hand-tracing `main.ts` → `AppModule`
- **Day 46:** Modules — create a `NotesModule` manually (not via CLI generator)
- **Day 47:** Controllers — write a `NotesController` with a GET endpoint
- **Day 48:** Controllers — GET endpoint with path params in NotesController
- **Day 49:** Rest / light review of Next.js to NestJS transition

## Week 8 — NestJS Providers, DI, & Review

- **Day 50:** Providers/Services — move logic into a `NotesService`, inject it into the controller
- **Day 51:** Dependency Injection — explain Dependency Injection out loud/in writing — why does Nest need `@Injectable()`?
- **Day 52:** POST endpoint — add a `create` method to service + controller
- **Day 53:** Review — rebuild the whole Notes module (controller/service) from blank files
- **Day 54:** Rebuild NestJS Notes module from memory — timed, no reference
- **Day 55:** DTOs — create `CreateNoteDto` with `class-validator` decorators
- **Day 56:** Rest / light review of NestJS dependency injection

## Week 9 — NestJS Validation & Database

- **Day 57:** Enable validation pipe globally, test that bad input gets rejected
- **Day 58:** Prisma setup — install Prisma, run prisma init
- **Day 59:** Prisma schema — set up a `Note` model, run a migration
- **Day 60:** Wire `NotesService` to the database for GET (read all)
- **Day 61:** Wire POST (create) to the database
- **Day 62:** Add PATCH and DELETE endpoints backed by the DB
- **Day 63:** Rest / light review of NestJS database integration

## Week 10 — NestJS CRUD Review & Integration

- **Day 64:** Rebuild the full CRUD resource from scratch, timed, no reference
- **Day 65:** Trace NestJS request lifecycle from controller to database and back
- **Day 66:** Point your Next.js app's fetch calls at your NestJS API (CORS setup)
- **Day 67:** CORS & error handling diagnostics on Next.js frontend
- **Day 68:** Basic auth — add a simple login endpoint in Nest (email/password, no JWT yet)
- **Day 69:** JWT — issue a token on login, write the auth service logic by hand
- **Day 70:** Rest / light review of Next.js and NestJS integration

## Week 11 — Auth guards, Protection & Integration

- **Day 71:** Protect a route with an auth guard — write the guard yourself
- **Day 72:** Protect route with auth guard — debug and test guard with expired tokens
- **Day 73:** Frontend — store token, attach it to authenticated fetch requests
- **Day 74:** Protected page — redirect unauthenticated users on the frontend
- **Day 75:** Review the full auth flow end-to-end, explain each step without notes
- **Day 76:** Rebuild auth endpoints and guard from memory
- **Day 77:** Rest / light review of authentication mechanics

## Week 12 — Solo Build (No AI, No Reference)

- **Day 78:** Plan a small full-stack app (e.g., task tracker) — routes, data model, pages, on paper
- **Day 79:** Build NestJS backend: module + controller + service skeleton
- **Day 80:** Backend: DB model + CRUD endpoints
- **Day 81:** Backend: auth (login + protected routes)
- **Day 82:** Frontend: pages + routing in Next.js
- **Day 83:** Frontend: connect to backend, forms, list views
- **Day 84:** Polish, fix bugs, and do a final self-check — could you rebuild this whole thing again from nothing?

---

## Rules for every session
1. Start from a blank file — don't open a template or reference first.
2. Try for the full 30-45 min before looking anything up.
3. Only after attempting, compare against docs or what AI would write — note the gap.
4. If a day's concept doesn't stick, repeat it before moving on rather than pushing forward on schedule.

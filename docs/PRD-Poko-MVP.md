
# Product Requirements Document: Poko MVP

## Executive Summary

**Product:** Poko

**Version:** MVP (1.0)

**Document Status:** Final Draft

**Last Updated:** February 12, 2026

### Product Vision

Poko is a "brain-dump to organized-timeline" productivity tool. It bridges the gap between the clinical feel of Todoist and the high learning curve of Notion. By prioritizing a **low-friction "Blurt" input** and a **high-aesthetic visual timeline**, Poko provides a neurodivergent-friendly experience without the paywalls found in competitors.

### Success Criteria

* **Onboarding:** Successfully recruit and onboard **10 beta testers**.
* **Engagement:** Users complete self-set tasks and open the app multiple times daily.
* **Utility:** High conversion from "Blurted" thoughts to completed tasks.

---

## Problem Statement

### Problem Definition

* **Entry Friction:** Complex apps take too long to set up, leading to "productivity procrastination."
* **Aesthetic Friction:** Standard managers are visually boring, failing to provide the "dopamine reward" needed by creative and ND users.
* **Economic Friction:** Many ADHD-specific productivity apps are hidden behind steep monthly paywalls.

---

## Target Audience

### Primary Persona: The Visual Academic / Creative

* **Who:** Students (e.g., UCI CSE) and creative pros who need to capture thoughts instantly.
* **The Struggle:** Losing ideas because the "Add Task" button requires too many fields (date, project, tags).
* **The Need:** A "pretty" interface that feels like a reward rather than a chore.

---

## User Journey: "The Blurt to Done"

1. **Discovery:** User hears about a "free, pretty ADHD-friendly app."
2. **The Blurt:** User opens Poko and "blurts" out 10 tasks in a single sitting without sorting.
3. **Organization:** Poko automatically categorizes these into a Low/Medium/High priority list.
4. **The Timeline:** User views these tasks on a beautiful, Tiimo-style timeline.
5. **Success:** User checks off a task, gets a visual reward, and returns later that day.

---

## MVP Features (MoSCoW)

### Must Have (P0) — *1.5 Week Build*

* **The "Blurt" Engine:** A rapid-fire input field where pressing 'Enter' instantly creates a task.
* **Priority Hierarchy:** A simple way to toggle tasks between Low, Medium, and High priority.
* **Aesthetic Timeline:** A visually pleasing vertical/horizontal day view with a curated color palette.
* **Task CRUD:** Basic ability to create, read, update, and delete tasks.

### Should Have (P1)

* **Mood Check-in:** A simple vibe-tracker emoji at the start of the session.
* **Completion Animation:** A "satisfying" visual pop when a task is completed.

### Won't Have (v1.0)

* External Calendar Sync (Google/Outlook).
* Collaborative/Shared lists.
* Complex Database relations.

---

## Technical Specifications

### The Stack

* **Backend:** FastAPI or Flask (Python) for rapid API development.
* **Frontend:** Next.js / React (TypeScript) for a snappy, interactive UI.
* **Styling:** Tailwind CSS + Framer Motion (for those "pretty" animations).
* **Database:** PostgreSQL (Supabase) or simple LocalStorage for the initial 10-day test.

### Non-Functional Requirements

* **Speed:** Task creation must feel instantaneous (<100ms UI update).
* **Mobile-First:** The "Blurt" input must be thumb-friendly for mobile users.
* **Design System:** Use consistent design tokens (colors, spacing) to ensure it looks "high-end."

---

## Risk Assessment

* **Timeline Risk:** 10 days is tight for a custom Timeline UI.
* **Mitigation:** Use a lightweight library for the timeline structure and spend time on the **CSS styling** to ensure the "aesthetic" requirement is met.

---

## MVP Definition of Done

* [ ] Users can "blurt" 5+ tasks in 30 seconds.
* [ ] Tasks are visually sorted by priority.
* [ ] Timeline view renders correctly on Mobile and Desktop.
* [ ] 10 Beta users have access to a live URL.

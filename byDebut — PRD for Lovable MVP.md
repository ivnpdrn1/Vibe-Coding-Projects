# byDebut — PRD for Lovable MVP

## Version 1.0 — Narrative Transformation Platform

---

# PRODUCT NAME

# byDebut

## “Change One Variable. Rewrite Everything.”

---

# PRODUCT VISION

byDebut is an AI-powered narrative transformation platform that allows readers to generate alternate versions of novels by modifying fundamental narrative variables such as immortality, religion, AI governance, memory, justice, war, power, love, or political systems.

The platform transforms passive reading into interactive narrative evolution.

Readers begin with an original novel and create private alternate versions while preserving thematic and narrative coherence through LLM-powered story transformation.

---

# CORE CONCEPT

Every published novel becomes:

* a canonical narrative,
* a transformation seed,
* and a launch point for infinite narrative variations.

The original novel remains protected intellectual property.

The platform only allows controlled narrative transformations and chapter-based evolution.

---

# MVP OBJECTIVE

Build the first production-ready version of byDebut using:

* [Lovable](https://lovable.dev?utm_source=chatgpt.com)
* [Supabase](https://supabase.com?utm_source=chatgpt.com)
* [OpenAI API](https://platform.openai.com?utm_source=chatgpt.com)

The MVP must:

* support user accounts,
* host novels,
* allow chapter-based transformations,
* generate alternate narrative versions,
* preserve narrative coherence,
* save private generations,
* prepare future scaling toward a narrative ecosystem.

---

# PRIMARY USER FLOW

## Step 1

Reader purchases/read novel on Amazon KDP.

---

## Step 2

Reader reaches final chapter:

# “BYDEBUT Chapter”

This chapter explains:

> This story does not end here.
> Go to byDebut.com and create your own version of this novel by changing one fundamental variable.

---

## Step 3

Reader scans QR code or enters byDebut.com.

---

## Step 4

Reader creates account.

---

## Step 5

Reader selects novel.

---

## Step 6

Reader chooses transformation mode.

Examples:

* Literary Mode
* Systemic Analysis Mode
* Cinematic Variation Mode
* Full Novel Evolution Mode

---

## Step 7

Reader selects transformation variable.

Examples:

* Immortality
* AI governance
* Memory permanence
* Religion collapse
* Justice system inversion
* Power centralization
* Elimination of death
* Eternal elites

---

## Step 8

LLM generates narrative variation.

---

## Step 9

User saves version to private library.

---

# MVP FEATURES

# 1. Landing Page

## Purpose

Introduce byDebut concept.

## Includes

* Hero section
* “Fork the Story”
* Explanation video placeholder
* Featured novels
* Public domain library
* Login / Signup
* CTA buttons

---

# 2. Authentication

## Technology

Supabase Auth.

## Required

* Email/password
* Google login
* Session persistence
* Password reset

---

# 3. User Dashboard

## Includes

* User library
* Saved variations
* Continue reading
* Recent generations
* Favorite universes

---

# 4. Novel Library

## Categories

### Public Domain

Examples:

* Les Misérables
* Dracula
* Frankenstein
* Don Quixote

### Premium Author Works

Examples:

* Eternidad Letal
* The Only Option
* Las Gargantas del Diablo

---

# 5. Novel Reader Interface

## Required

* Chapter-based reading
* Protected rendering
* Disable raw copy/download
* Reader mode
* Dark/light theme

---

# 6. Transformation Engine

## Core MVP Feature

User selects:

* narrative variable,
* transformation mode,
* chapter scope.

Then system generates alternate narrative continuation.

---

# 7. Transformation Modes

# Literary Mode

Focus:

* prose quality,
* emotional coherence,
* literary continuity.

---

# Systemic Analysis Mode

Focus:

* political,
* philosophical,
* societal consequences.

---

# Cinematic Variation Mode

Focus:

* visual scenes,
* pacing,
* dramatic tension.

---

# Full Novel Evolution Mode

Focus:

* long-term narrative divergence.

---

# 8. Private Version Library

Each user has:

* saved branches,
* generated timelines,
* alternate versions,
* narrative history.

---

# 9. QR Entry System

Each Amazon novel includes:

* QR code,
* direct novel onboarding link.

Example:

```text id="df4v9x"
bydebut.com/eternidad-letal
```

---

# 10. AI Narrative Coherence System

The system must:

* preserve character consistency,
* maintain timeline continuity,
* preserve tone,
* preserve worldbuilding,
* prevent contradiction collapse.

---

# TECH STACK

# Frontend

## Platform

Lovable

## Framework

React + Tailwind

---

# Backend

## Supabase

Includes:

* PostgreSQL
* Authentication
* Storage
* Edge Functions

---

# AI Layer

## Phase 1

OpenAI API

Recommended:

* GPT-5 class reasoning model
* long-context support

---

## Phase 2

Gemini API integration

Used for:

* multimodal reasoning,
* large-context processing,
* cinematic analysis.

---

# DATABASE STRUCTURE

# USERS

```sql id="jv6b89"
users
- id
- email
- created_at
```

---

# NOVELS

```sql id="wq7r5k"
novels
- id
- title
- author
- description
- public_domain
- premium
- cover_image
```

---

# CHAPTERS

```sql id="m1q3wr"
chapters
- id
- novel_id
- chapter_number
- title
- content
```

---

# GENERATIONS

```sql id="l3zq8n"
generations
- id
- user_id
- novel_id
- source_chapter
- transformation_variable
- mode
- generated_content
- created_at
```

---

# SAVED UNIVERSES

```sql id="0hzn73"
universes
- id
- user_id
- title
- description
- root_generation_id
```

---

# SECURITY REQUIREMENTS

# Critical

The platform MUST NOT:

* expose full original novel downloads,
* expose raw text exports,
* allow scraping,
* allow unrestricted copy.

---

# Required Protections

* chapter rendering only,
* partial loading,
* rate limiting,
* generation quotas,
* API protection,
* signed access URLs.

---

# AI PROMPTING ARCHITECTURE

# System Prompt Layer

Defines:

* literary continuity,
* tone preservation,
* narrative coherence,
* forbidden contradictions.

---

# Transformation Prompt Layer

Injects:

* selected variable,
* transformation style,
* narrative scope.

---

# Context Retrieval Layer

Uses:

* chapter embeddings,
* narrative memory,
* character state tracking.

---

# FUTURE FEATURES

# Phase 2

* Community forks
* Public universes
* Voting/ranking
* Narrative branching visualization
* Story graph
* Timeline explorer

---

# Phase 3

* AI voice narration
* Cinematic scene generation
* AI-generated trailers
* Multi-author collaborative universes

---

# PHASE 4

* “GitHub for Narrative Universes”
* Pull requests for story branches
* Canon timelines
* Alternate civilization simulations

---

# LOVABLE IMPLEMENTATION PLAN

# Phase 1 — UI Foundation

Build:

* landing page,
* login,
* dashboard,
* library,
* reader UI.

---

# Phase 2 — Supabase Integration

Implement:

* auth,
* database,
* storage,
* session persistence.

---

# Phase 3 — OpenAI Integration

Implement:

* narrative generation,
* prompt orchestration,
* chapter transformation.

---

# Phase 4 — Narrative Memory

Implement:

* embeddings,
* retrieval,
* continuity preservation.

---

# Phase 5 — Cursor Refactoring

Move to:

* production-grade structure,
* security hardening,
* API optimization,
* cost control,
* deployment preparation.

---

# SUCCESS METRICS

# MVP Success

* users generate alternate versions,
* users save private universes,
* narrative coherence maintained,
* readers return after Amazon purchase.

---

# Long-Term Success

byDebut becomes:

# “The platform where stories evolve.”

---

# FINAL POSITIONING

byDebut is not merely an AI writing platform.

It is:

# a narrative transformation engine

# for evolving stories, civilizations, and ideas through AI-assisted alternate realities.

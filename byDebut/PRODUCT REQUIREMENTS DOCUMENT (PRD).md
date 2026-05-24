# PRODUCT REQUIREMENTS DOCUMENT (PRD)

# byDebut

## The Story Transformation Engine

Version: 1.0
Prepared For: [Lovable](https://lovable.dev?utm_source=chatgpt.com)
Founder: Iván Padrón
Product Type: AI Narrative Transformation Platform
Target Release: MVP → Scalable Public Platform

---

# 1. PRODUCT OVERVIEW

## Product Name

byDebut

---

## Core Vision

byDebut transforms books from static reading experiences into evolving narrative systems.

Readers can:

* select a book,
* modify a central variable,
* generate alternative narrative realities,
* create new story branches,
* explore consequences,
* publish variations,
* vote on versions,
* and participate in collaborative narrative evolution.

The platform combines:

* AI narrative generation,
* speculative storytelling,
* branching narrative systems,
* reader participation,
* and structured literary transformation.

---

# 2. CORE PRODUCT CONCEPT

Traditional books end.

byDebut allows stories to continue evolving.

Every book becomes:

* a narrative universe,
* a system of variables,
* and a generator of alternate realities.

The user changes one variable.

The AI builds a new version of the story.

---

# 3. PRIMARY GOALS

## MVP Goals

### Goal 1

Launch a functional public platform where users can:

* browse books,
* create account,
* select a book,
* modify a variable,
* generate a new premise,
* save variations,
* and publish/share versions.

---

### Goal 2

Create a viral “story transformation” mechanic.

---

### Goal 3

Position byDebut as:

> “The first narrative transformation platform.”

---

### Goal 4

Create scalable infrastructure for future expansion:

* full chapter generation,
* cinematic adaptation generation,
* AI narrative simulation,
* collaborative worldbuilding,
* creator monetization.

---

# 4. TARGET USERS

## Primary Audience

### Speculative Fiction Readers

Users interested in:

* sci-fi,
* dystopian fiction,
* philosophy,
* alternate history,
* AI futures,
* geopolitical fiction.

---

## Secondary Audience

### Writers

Users who want:

* idea generation,
* branching story development,
* worldbuilding,
* narrative experimentation.

---

## Third Audience

### Film / TV / Gaming Creators

Users looking for:

* new narrative concepts,
* adaptable IP,
* audience-validated ideas.

---

# 5. MARKET POSITIONING

byDebut is NOT:

* fan fiction,
* generic AI writing,
* prompt playground,
* chatbot storytelling.

byDebut IS:

* structured narrative transformation,
* variable-driven storytelling,
* civilization-level speculative simulation,
* collaborative narrative evolution.

---

# 6. CORE USER FLOW

# MASTER FLOW

```text
User visits byDebut
↓
Creates account
↓
Explores books
↓
Selects a book
↓
Reads original premise
↓
Selects variable to modify
↓
Writes modification idea
↓
AI generates new premise
↓
User saves variation
↓
Variation becomes public/private
↓
Community votes/ranks
↓
Other users fork variations
↓
Narrative tree expands
```

---

# 7. INFORMATION ARCHITECTURE

# PUBLIC ROUTES

```text
/
```

Landing page

```text
/books
```

Books library

```text
/book/[slug]
```

Book detail page

```text
/version/[slug]
```

Generated variation page

```text
/user/[username]
```

User profile

```text
/rankings
```

Top variations

```text
/explore
```

Narrative exploration

---

# AUTH ROUTES

```text
/login
/signup
/account
```

---

# CREATION ROUTES

```text
/book/[slug]/create
```

```text
/version/[id]/fork
```

---

# 8. CORE FEATURES

# FEATURE 1 — BOOK PAGES

Each book page must include:

* cover,
* title,
* author,
* synopsis,
* central variable,
* themes,
* “Create New Version” CTA,
* public variations,
* top ranked variations.

---

# FEATURE 2 — VARIABLE MODIFICATION ENGINE

User selects:

* variable type,
* narrative change,
* philosophical shift,
* political shift,
* emotional change,
* technological alteration.

Examples:

```text
“What if immortality existed only for the wealthy?”
“What if AI replaced democracy?”
“What if memory could be edited?”
```

---

# FEATURE 3 — AI PREMISE GENERATION

AI generates:

* transformed premise,
* narrative consequences,
* story direction,
* civilization impact,
* emotional tone.

---

# FEATURE 4 — VERSION SYSTEM

Each generated variation becomes:

* independent page,
* shareable URL,
* forkable narrative node.

Example:

```text
/version/immortality-for-the-rich
```

---

# FEATURE 5 — FORK SYSTEM

Users can create variations from other variations.

This creates narrative trees.

---

# FEATURE 6 — RANKING SYSTEM

Users can:

* vote,
* favorite,
* follow,
* rank variations.

Possible ranking categories:

* Most Philosophical
* Most Cinematic
* Most Realistic
* Most Dangerous
* Most Original

---

# FEATURE 7 — USER PROFILES

Each user profile includes:

* created versions,
* followers,
* rankings,
* saved worlds,
* favorite books.

---

# FEATURE 8 — PRIVATE/PUBLIC MODE

Users can choose:

* private draft,
* public version,
* collaborative mode.

---

# FEATURE 9 — AI CHAPTER GENERATION (PHASE 2)

Future expansion:

* chapter generation,
* full books,
* screenplay mode,
* cinematic pitch mode.

---

# 9. MVP SCOPE

# INCLUDED IN MVP

✅ Landing page
✅ Auth
✅ Book library
✅ Book detail pages
✅ Variable selection
✅ AI premise generation
✅ Save variation
✅ Public/private versions
✅ Ranking system
✅ User profiles
✅ Forking system
✅ Responsive design

---

# EXCLUDED FROM MVP

❌ Full novel generation
❌ Marketplace
❌ Payments
❌ Multi-language AI generation
❌ Mobile app
❌ Advanced cinematic exports
❌ Real-time collaboration

---

# 10. RECOMMENDED TECH STACK

# FRONTEND

Generated via Lovable:

* React
* Next.js
* TailwindCSS

---

# HOSTING

Recommended:

* Vercel

---

# BACKEND

Recommended:

* [Supabase](https://supabase.com?utm_source=chatgpt.com)

Including:

* PostgreSQL
* Auth
* Edge Functions
* Storage
* Realtime

---

# AI PROVIDERS

Primary:

* [OpenAI](https://openai.com?utm_source=chatgpt.com)

Future:

* [Anthropic](https://www.anthropic.com?utm_source=chatgpt.com)
* [Google Gemini](https://gemini.google.com?utm_source=chatgpt.com)

---

# CODE REPOSITORY

* [GitHub](https://github.com?utm_source=chatgpt.com)

---

# ANALYTICS

Recommended:

* PostHog
* GA4

---

# DOMAIN

```text
bydebut.com
```

---

# 11. DATABASE ARCHITECTURE

# TABLE: users

```text
id
username
email
bio
avatar_url
created_at
```

---

# TABLE: books

```text
id
title
slug
author
description
cover_url
central_variable
copyright_status
amazon_url
public_domain
created_by
created_at
```

---

# TABLE: variables

```text
id
book_id
name
description
example_prompt
```

---

# TABLE: versions

```text
id
book_id
parent_version_id
user_id
title
slug
modified_variable
premise
synopsis
visibility
votes
created_at
```

---

# TABLE: chapters

```text
id
version_id
chapter_number
title
content
created_at
```

---

# TABLE: votes

```text
id
user_id
version_id
vote_type
created_at
```

---

# TABLE: forks

```text
id
parent_version_id
child_version_id
created_at
```

---

# 12. AI GENERATION FLOW

```text
User modifies variable
↓
System sends structured prompt
↓
AI generates:
   - premise
   - consequences
   - emotional tone
   - world changes
↓
Result displayed
↓
User edits/accepts
↓
Version saved
```

---

# 13. PROMPT ENGINEERING STRATEGY

Prompts must enforce:

* narrative consistency,
* philosophical depth,
* civilization-level consequences,
* emotional realism,
* speculative sophistication.

The AI should NOT produce:

* random fanfiction,
* disconnected scenes,
* generic chatbot outputs.

---

# 14. CONTENT SAFETY

System must prevent:

* illegal content,
* explicit abuse,
* hateful extremism,
* plagiarism,
* copyrighted reproduction.

Public domain works allowed.

User-owned books allowed.

---

# 15. UX PRINCIPLES

# RULE 1

Simple enough for non-technical readers.

---

# RULE 2

Creation flow must feel magical but controlled.

---

# RULE 3

Narrative transformation must be understandable in under 60 seconds.

---

# RULE 4

Every page must communicate:

> “Change one variable. Create a new world.”

---

# 16. LANDING PAGE STRUCTURE

# HERO SECTION

Headline:

```text
Every Story Can Become Another Civilization
```

Subheadline:

```text
Change one variable.
Create a new version.
Explore the consequences.
```

CTA:

```text
Start Exploring
```

---

# HOW IT WORKS SECTION

```text
1. Choose a book
2. Change a variable
3. Generate a new version
4. Explore alternate realities
```

---

# SOCIAL PROOF SECTION

Future:

* top creators,
* top worlds,
* most cinematic variations.

---

# 17. SCALABILITY PLAN

# PHASE 1

Premise generation

---

# PHASE 2

Chapter generation

---

# PHASE 3

Complete novels

---

# PHASE 4

Screenplay generation

---

# PHASE 5

Collaborative universes

---

# PHASE 6

Creator monetization

---

# 18. MONETIZATION FUTURE

Possible models:

* premium generations,
* creator subscriptions,
* cinematic pitch exports,
* AI narrative credits,
* marketplace,
* publisher partnerships.

---

# 19. DIFFERENTIATION

Unlike generic AI writing tools:

byDebut is built around:

* books,
* narrative variables,
* branching realities,
* philosophical consequences,
* civilization-level storytelling.

This is not “AI writes text.”

This is:

> “AI transforms worlds.”

---

# 20. SUCCESS METRICS

# MVP Metrics

* Account creation rate
* Story creation rate
* Average session duration
* Fork rate
* Public sharing rate
* Returning users
* Variations per book
* Community voting activity

---

# 21. FINAL PRODUCT VISION

byDebut becomes:

* a narrative operating system,
* a civilization simulator through fiction,
* an AI-powered literary ecosystem,
* and a new category between:

  * publishing,
  * gaming,
  * storytelling,
  * and speculative simulation.

---

# FINAL PRODUCT STATEMENT

> byDebut transforms books from finished stories into living narrative universes that readers can evolve, modify, and expand through AI-powered variable transformation.

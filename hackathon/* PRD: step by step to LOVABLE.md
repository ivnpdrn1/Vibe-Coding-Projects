# STEP 1 — CREATE THE PROJECT IN LOVABLE

Copy and paste this FIRST into Lovable:

```text
Create a new project called byDebut.

byDebut is NOT a generic AI writing app.

byDebut is an AI-powered reader engagement platform for independent authors.

The platform transforms books into interactive narrative ecosystems where readers can modify one variable from a story and generate alternate realities using AI.

The goal is to increase reader engagement after finishing a book.

Core concept:

Reader finishes a novel
↓
Reader enters byDebut
↓
Reader changes ONE variable
↓
AI generates an alternate world
↓
Reader saves and shares the variation

IMPORTANT:

Do NOT redesign the product.
Do NOT simplify the positioning.
Do NOT convert this into a chatbot or generic storytelling app.
Do NOT introduce unrelated SaaS productivity features.

The platform must feel:
- cinematic
- immersive
- speculative
- emotional
- modern

The interface must be understandable within 60 seconds.

Core product message:

"Change one variable. Create a new world."
```

---

# STEP 2 — BUILD THE FRONTEND MVP ONLY

After Lovable creates the project, copy and paste this:

```text
Build ONLY the frontend MVP structure first.

Do NOT implement advanced backend logic yet.

Create these pages:

1. Landing Page
2. Login / Signup
3. Books Library
4. Individual Book Page
5. Variable Transformation Interface
6. Public Variations Gallery

UI STYLE REQUIREMENTS:

The UI must feel:
- premium
- cinematic
- emotionally immersive
- speculative sci-fi inspired
- NOT corporate SaaS

Avoid:
- generic dashboards
- productivity app appearance
- chatbot layouts

Landing page hero section:

Headline:
"Every Book Can Become Another World"

Subheadline:
"Change one variable. Generate a new reality. Explore the consequences."

CTA Button:
"Start Exploring"

The homepage must visually explain this flow:

1. Choose a book
2. Change one variable
3. AI generates a new world
4. Share the variation

IMPORTANT:
Focus ONLY on frontend structure and beautiful UX.
Do NOT build advanced features yet.
```

---

# STEP 3 — CREATE THE BOOK PAGE EXPERIENCE

After frontend pages exist, paste this:

```text
Now improve the individual book page experience.

Create a cinematic book universe page.

Example route:
/book/eternidad-letal

The page must include:

- large book cover
- title
- synopsis
- central story variable
- immersive atmosphere
- "Change a Variable" section
- existing public variations

IMPORTANT:

The emotional focus must be:
"What happens if this changes?"

Add a prominent transformation input box.

Example placeholder text:

"What if immortality only existed for the wealthy?"

Add a large CTA button:
"Generate Alternate World"

The page must feel like entering a narrative universe.
```

---

# STEP 4 — BUILD THE VARIABLE TRANSFORMATION FLOW

Paste this next:

```text
Now build the core transformation flow.

User Flow:

1. User selects a book
2. User types one variable change
3. User clicks "Generate Alternate World"
4. AI response area appears
5. User can save or share the variation

IMPORTANT:

This is the CORE LOOP of the platform.

The experience must feel:
- immediate
- magical
- emotionally engaging
- simple

Do NOT overload the interface.

The generated result area must include:

- Alternate World Title
- Premise
- Social Consequences
- Emotional Consequences
- Civilization Impact

Keep the UX clean and cinematic.
```

---

# STEP 5 — CONNECT SUPABASE

Paste this AFTER the UI exists:

```text
Now integrate Supabase as the backend.

Requirements:

Authentication:
- email signup
- login
- session persistence

Database tables:

users
books
variations

Books table fields:
- id
- title
- slug
- description
- cover_url

Variations table fields:
- id
- book_id
- user_id
- modified_variable
- generated_world
- created_at

Implement:
- save variations
- load public variations
- associate variations with users

IMPORTANT:
Keep backend architecture simple and scalable.
```

---

# STEP 6 — CONNECT GEMINI API

Paste this AFTER Supabase works:

```text
Now integrate Gemini API as the PRIMARY AI engine.

Gemini will power:
- alternate world generation
- consequence generation
- narrative transformation

IMPORTANT:
Gemini is mandatory and must remain the primary AI provider.

When a user changes a variable, Gemini should generate:

1. Alternate World Title
2. New Premise
3. Social Consequences
4. Emotional Consequences
5. Civilization-Level Impact

The outputs must feel:
- intelligent
- speculative
- cinematic
- emotionally coherent

Avoid generic chatbot responses.

The response should feel like a transformed civilization.
```

---

# STEP 7 — BUILD PUBLIC GALLERY

Paste this next:

```text
Now create the Public Variations Gallery.

Page route:
/explore

Show:
- latest variations
- featured worlds
- trending alternate realities

Each card should include:
- book title
- modified variable
- generated world title
- short premise preview

Each variation must link to:
'/version/[slug]'

IMPORTANT:
This page should feel like exploring alternate civilizations.
Not social media.
```

---

# STEP 8 — BUILD VERSION PAGES

Paste this next:

```text
Now create individual variation pages.

Example route:
/version/immortality-for-the-rich

Each page must include:

- original book reference
- modified variable
- generated alternate world
- consequences
- creation date
- creator username

Add buttons:
- Share
- Create Another Variation

IMPORTANT:
The page must feel like a discovered alternate reality.
```

---

# STEP 9 — ADD AI MODERATION

Paste this next:

```text
Now implement AI moderation.

The system must automatically detect:
- abusive content
- hate content
- illegal content
- spam
- unsafe outputs

Create an AI moderation layer before publishing variations.

Add moderation logs to the admin backend.

IMPORTANT:
Moderation should happen automatically and invisibly.
```

---

# STEP 10 — ADD STRIPE PAYMENTS

Paste this next:

```text
Now integrate Stripe payments.

Create two plans:

Creator Plan:
$9/month

Pro Plan:
$29/month

Features can remain placeholder initially.

The purpose is to:
- demonstrate real business capability
- support hackathon revenue requirements

Create:
- pricing page
- subscription flow
- upgrade buttons
- billing success/cancel pages

IMPORTANT:
Keep payments simple and production-ready.
```

---

# STEP 11 — BUILD AUTHOR DASHBOARD

Paste this next:

```text
Now create the Author Dashboard.

Authors should see:

- books uploaded
- total variations created
- reader engagement
- most modified variables
- recent activity

The dashboard must feel:
- clean
- modern
- creator-focused

Avoid enterprise SaaS complexity.

IMPORTANT:
This dashboard demonstrates business viability for the hackathon.
```

---

# STEP 12 — BUILD AI OPERATIONS DASHBOARD

Paste this LAST:

```text
Now create an AI Operations Dashboard for hackathon demonstration purposes.

Show:
- Gemini generation logs
- moderation events
- AI classifications
- total AI generations
- active users
- variation creation activity

This dashboard exists to visually demonstrate:
"AI operating the business"

IMPORTANT:
The dashboard should look real, modern, and production-ready.
This is critical for the hackathon demo video.
```

Aquí tienes la **secuencia completa**, lista para copiar y pegar en Lovable **bloque por bloque**.

---

# BLOQUE 1 — Crear proyecto

```text
Create a new project called byDebut.

byDebut is an AI-native narrative creator economy platform.

It is NOT:
- a generic AI writing assistant
- a chatbot
- a fanfiction website
- a productivity SaaS app

Core concept:
A user selects a book, changes one important variable in the story, and Gemini generates an alternate world with audience prediction and marketing guidance.

Primary message:
"Change one variable. Create a new world."

The product must feel:
- cinematic
- emotional
- modern
- immersive
- simple to understand

Do not redesign the product.
Do not change the positioning.
Do not add unrelated features.
Do not overbuild.

Build only what is requested step by step.
```

---

# BLOQUE 2 — Tipos de usuarios y suscripciones

```text
Define the official user types and subscription model for byDebut.

USER TYPE 1 — EXPLORER

Subscription:
Free

Purpose:
Readers exploring alternate worlds.

Capabilities:
- browse books
- explore public worlds
- create limited variations
- share public links

Limitations:
- limited AI generations per month
- no advanced analytics
- no creator branding

---

USER TYPE 2 — CREATOR

Subscription:
$5/month

Purpose:
Readers becoming narrative creators.

Capabilities:
- higher AI generation limits
- creator profile
- public creator page
- audience interest predictions
- marketing recommendations
- public publishing
- creator dashboard

This is the primary growth user type.

---

USER TYPE 3 — PRO CREATOR

Subscription:
$15/month

Purpose:
Advanced creators building audiences and narrative brands.

Capabilities:
- very high AI generation limits
- advanced audience analysis
- advanced marketing guidance
- export tools
- premium creator branding
- analytics dashboard
- priority AI processing

---

IMPORTANT PRODUCT RULE:

The platform must encourage this evolution:

Reader
↓
Explorer
↓
Creator
↓
Audience Builder

The primary economic engine of byDebut is not authors alone.

The primary economic engine is large-scale narrative creators emerging from readers.
```

---

# BLOQUE 3 — Frontend MVP

```text
Build only the frontend MVP first.

Create these pages:

1. Landing Page
2. Login / Signup
3. Books Library
4. Individual Book Page
5. Variable Transformation Page
6. Public Variations Gallery
7. Individual Version Page
8. Pricing Page
9. Creator Dashboard

Do not connect backend yet.
Do not connect Gemini yet.
Do not connect Stripe yet.

Landing Page headline:
"Every Story Can Become Another World"

Subheadline:
"Change one variable. Generate a new reality. Discover the audience for your world."

CTA:
"Start Exploring"

Show this simple process visually:

1. Choose a book
2. Change one variable
3. Gemini generates an alternate world
4. AI predicts audience interest
5. Share your version

The design must be cinematic, premium, immersive, and simple.

Avoid:
- generic SaaS dashboards
- chatbot layouts
- productivity app appearance
```

---

# BLOQUE 4 — Página de libro

```text
Improve the individual book page.

Route example:
/book/eternidad-letal

Each book page must include:

- book cover
- title
- author
- synopsis
- central story variable
- themes
- public variations
- main CTA: "Change a Variable"

The emotional question on the page must be:
"What happens if this changes?"

Add a large input box with placeholder:
"What if immortality only existed for billionaires?"

Add button:
"Generate Alternate World"

The page must feel like entering a narrative universe.
```

---

# BLOQUE 5 — Flujo de transformación

```text
Build the core variable transformation flow.

User flow:

1. User selects a book
2. User types one variable change
3. User clicks "Generate Alternate World"
4. A generated result area appears
5. User can save, publish, or share the version

The generated result area must include:

- Alternate World Title
- New Premise
- Social Consequences
- Emotional Consequences
- Civilization-Level Impact
- Audience Interest
- Suggested Positioning
- Suggested Marketing Strategy

Keep the UX simple, cinematic, and emotionally engaging.

This is the core loop of byDebut.
Do not complicate it.
```

---

# BLOQUE 6 — Supabase

```text
Now integrate Supabase.

Use Supabase for:
- authentication
- database
- saving variations
- loading public gallery
- user roles
- subscription status

Create these tables:

users:
- id
- username
- email
- role
- subscription_plan
- created_at

books:
- id
- title
- slug
- author
- description
- cover_url
- central_variable
- created_at

variations:
- id
- book_id
- user_id
- title
- modified_variable
- generated_world
- audience_prediction
- marketing_suggestions
- visibility
- created_at

ai_logs:
- id
- agent_type
- action
- input_summary
- output_summary
- created_at

subscriptions:
- id
- user_id
- plan
- status
- stripe_customer_id
- created_at

Implement:
- signup
- login
- session persistence
- save variation
- publish variation
- load public variations
- user subscription state
```

---

# BLOQUE 7 — Gemini API

```text
Now integrate Gemini API as the primary AI engine.

Gemini must generate the full alternate world response.

When the user enters a variable change, Gemini must return:

1. Alternate World Title
2. New Premise
3. Social Consequences
4. Emotional Consequences
5. Civilization-Level Impact
6. Audience Interest Prediction
7. Suggested Positioning
8. Suggested Marketing Strategy

The output must feel:
- cinematic
- intelligent
- speculative
- emotionally coherent
- market-aware

Do not produce generic chatbot responses.

Prompting rule:
Gemini is not just writing a story.
Gemini is generating a market-aware alternate narrative world.
```

---

# BLOQUE 8 — Multi-agent Gemini logic

```text
Improve the AI output so it acts like multiple specialized AI agents.

Use Gemini to simulate these roles:

1. Narrative Generator
Creates the alternate world.

2. Audience Analyst
Predicts likely interested audiences.

3. Market Positioning Strategist
Suggests the best genre and positioning.

4. Marketing Advisor
Suggests how the creator should promote the version.

5. Moderation Agent
Flags unsafe or abusive content.

The user should see only the useful final output:

- generated world
- likely audience
- positioning
- marketing strategy

Save AI activity into the ai_logs table.
```

---

# BLOQUE 9 — Public Gallery

```text
Create the Public Variations Gallery.

Route:
/explore

Show public variations as cinematic cards.

Each card must show:

- original book title
- generated world title
- modified variable
- short premise preview
- audience fit label
- creator username

Each card links to:
/version/[slug]

The gallery must feel like exploring alternate worlds, not social media.
```

---

# BLOQUE 10 — Version page

```text
Create individual version pages.

Route example:
/version/immortality-for-billionaires

Each version page must show:

- original book
- creator username
- modified variable
- alternate world title
- generated premise
- social consequences
- emotional consequences
- civilization impact
- audience interest prediction
- suggested positioning
- suggested marketing strategy

Add buttons:
- Share Version
- Create Another Version
- Explore More Worlds

The page must feel like a complete narrative concept ready to be promoted.
```

---

# BLOQUE 11 — Pricing + Stripe

```text
Now create pricing and Stripe payment flow.

Create three plans:

Explorer:
Free

Creator:
$5/month

Pro Creator:
$15/month

Creator Plan includes:
- more AI generations
- creator profile
- public creator page
- audience insights
- marketing recommendations

Pro Creator includes:
- very high AI generation limits
- advanced positioning analysis
- advanced marketing recommendations
- export tools
- premium creator branding
- analytics dashboard

Create pages:
- /pricing
- checkout flow
- success page
- cancel page

Keep the payment system simple.
The purpose is to demonstrate real business and real revenue potential.
```

---

# BLOQUE 12 — Creator Dashboard

```text
Create a Creator Dashboard.

Route:
/dashboard

Show:

- subscription plan
- total versions created
- public versions
- saved drafts
- most used variables
- most promising audience segments
- recent AI generations
- upgrade CTA

Add a section:
"AI Growth Recommendations"

This section should show recommendations such as:

- best audience for this creator
- suggested social platform
- recommended content format
- strongest genre positioning
- next version idea with higher audience potential

The dashboard must feel like a creator growth studio, not a corporate admin panel.
```

---

# BLOQUE 13 — AI Operations Dashboard

```text
Create an AI Operations Dashboard for hackathon demonstration.

Route:
/admin/ai-ops

Show:

- total Gemini generations
- audience analysis events
- marketing recommendation events
- moderation events
- latest AI logs
- total active users
- total public variations
- subscription plan breakdown

Purpose:
This page demonstrates that AI is operating the business in production.

Make it visually clear and credible for hackathon judges.
```

---

# BLOQUE 14 — Demo data

```text
Add demo seed data for initial testing.

Create 3 sample books:

1. Eternidad Letal
Central variable:
Immortality

2. The Only Option
Central variable:
AI governance

3. The Devil's Throats
Central variable:
Global chokepoints

Add sample public variations for each book.

Make the demo feel real and ready for a 3-minute hackathon video.
```

---

# BLOQUE 15 — Final polish

```text
Polish the full MVP for hackathon presentation.

Prioritize:

- clear landing page
- smooth core loop
- beautiful book pages
- high-quality Gemini output
- audience prediction
- marketing recommendations
- public gallery
- creator dashboard
- AI operations dashboard
- Stripe pricing page

Do not add new major features.

Focus on making the existing experience feel complete, credible, and production-ready.
```

---

Después de pegar el **Bloque 1**, muéstrame la respuesta de Lovable antes de avanzar al Bloque 2.

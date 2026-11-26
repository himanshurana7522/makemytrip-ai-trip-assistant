
# Product Research — MakeMyTrip AI Trip Assistant

## 1. Research Overview

**Research objective:** Understand traveller planning problems, evaluate existing travel-planning experiences, and identify a product opportunity for a trust-aware AI trip assistant.

**Core problem:** Travel information is scattered across multiple sources, while generic recommendations can be difficult to trust.

**Research approach documented in the original assignment:**
- Proto-persona development
- Empathy mapping and AEIOU analysis
- Competitive teardown
- SWOT analysis
- Feature opportunity identification
- RICE prioritisation

**Important:** Aarav and Riya are proto-personas, not personas validated through documented user interviews.

---

## 2. Proto-Personas

### Primary Persona — Aarav Mehta

**Archetype:** The Time-Constrained Trip Planner

| Attribute | Details |
|---|---|
| Age | 27 |
| Location | Bengaluru |
| Occupation | Working professional |
| Travel pattern | Short trips when leave is available |
| Planning goal | Plan a 4–6 day trip quickly |
| Budget need | Stay within a defined budget |
| Interests | Find activities matching personal interests |

**Behaviours**
- Compares travel websites.
- Checks Google Maps.
- Saves social-media posts.
- Reads reviews.
- Drafts itineraries in Notes.

**Pain points**
- Travel information is scattered across sources.
- Popular recommendations may not match his budget or interests.
- Comparing several sources takes time.

**Expressed need:** A personalised itinerary that fits his budget and interests.

**Latent need:** Confidence in understanding why a recommendation suits him before acting on it.

**Persona insight:** Aarav wants faster planning but does not fully trust generic recommendations. His workaround is to check several sources and build his own plan.

### Secondary Persona — Riya Sharma

**Archetype:** The Risk-Conscious Family Trip Planner

| Attribute | Details |
|---|---|
| Age | 35 |
| Location | Delhi |
| Occupation | Working professional |
| Travel pattern | Family holidays |
| Planning goal | Comfortable trips suitable for different age groups |
| Budget need | Manage family-trip spending |

**Behaviours**
- Reads reviews.
- Checks hotel facilities and locations.
- Consults family members.
- Keeps backup options.

**Pain points**
- A high rating does not necessarily mean a hotel or activity suits her family.
- Rechecking options across multiple sources adds planning effort.

**Expressed need:** A safe, comfortable and family-friendly itinerary.

**Latent need:** Reassurance that important family requirements have not been overlooked.

**Persona insight:** Riya wants simple planning but checks options repeatedly because she feels responsible for everyone's comfort.

---

## 3. Competitive Teardown

The original assessment compared three travel-planning experiences.

| Capability | MakeMyTrip / Myra | Wanderlog | Google Gemini / Maps |
|---|---|---|---|
| Conversational planning | Yes | Yes | Yes |
| Personalised itinerary | Yes | Yes | Yes |
| Hotel suggestions | MMT marketplace | Yes | Google Hotels / connected sources |
| Activity suggestions | Yes | Yes | Yes |
| Route-aware planning | Travel ecosystem context | Strong route optimisation | Strong map context |
| Booking journey | Strong MMT marketplace link | Planning and reservation tools | Varies by workflow |
| Trip collaboration | Not its main focus | Core feature | Sharing, not a dedicated group planner |
| Offline access | Not its main focus | Available | Offline Maps |
| Recommendation rationale | Opportunity for this case | Review-backed suggestions | Personal context |

### Competitive Insights

**MakeMyTrip / Myra**
- Has an existing travel marketplace.
- Can potentially connect planning with booking.
- Personalisation alone does not guarantee recommendation fit.

**Wanderlog**
- Strong in route planning.
- Supports trip organisation and collaboration.
- Offers offline access.

**Google Gemini / Maps**
- Combines travel information with Maps and personal context.
- Provides strong place-discovery capabilities.

### Identified Product Opportunity

Basic itinerary generation is becoming common.

The proposed differentiator is:
- Explain why recommendations may suit the traveller.
- Make budget and preference fit visible.
- Clearly communicate uncertainty.
- Avoid treating popularity as a substitute for relevance.

*Note: This is the competitor assessment documented in the original assignment, not a newly conducted live competitor audit.*

---

## 4. SWOT Analysis — MakeMyTrip

### Strengths
- Existing travel marketplace.
- AI assistant planning can connect with the booking ecosystem.
- Potential to convert trip-planning activity into transactions.

### Weaknesses
- Personalisation does not automatically ensure that recommendations match actual traveller needs.

### Opportunities
- Use stated preferences, budget and trip context.
- Improve recommendation relevance.
- Explain why suggestions may fit.
- Build user trust through visible uncertainty.

### Threats
- Popular destinations may dominate recommendations.
- Expensive options may receive disproportionate attention.
- Highly reviewed or geographically concentrated options may dominate unless ranking and evaluation check for these biases.

### SWOT Conclusion

MakeMyTrip's marketplace provides a potential booking advantage. However, the opportunity identified in this project is to improve recommendation relevance and trust rather than simply generate another itinerary.

---

## 5. Feature Opportunity Backlog

| Opportunity | Description | Target Persona |
|---|---|---|
| Smart Itinerary Generator | Creates a day-by-day plan from destination, dates, budget and interests. | Aarav |
| Conversational Trip Planner | Asks follow-up questions before creating a plan. | Aarav |
| Trust-Aware Itinerary Assistant | Explains why suggestions may fit and considers recommendation-bias risks. | Aarav |
| Family-Safe Trip Planner | Considers age groups, family needs, distance and rest time. | Riya |

---

## 6. RICE Prioritisation

**Formula:**

RICE = (Reach × Impact × Confidence) ÷ Effort

For this exercise:
- Reach: Relative score from 1–10
- Impact: Score from 1–5
- Confidence: Decimal value
- Effort: Score from 1–10

| Feature | Reach | Impact | Confidence | Effort | RICE Score |
|---|---:|---:|---:|---:|---:|
| Smart Itinerary Generator | 9 | 3 | 0.90 | 3 | 8.10 |
| Conversational Trip Planner | 8 | 4 | 0.85 | 5 | 5.44 |
| Trust-Aware Assistant | 10 | 5 | 0.90 | 4 | 11.25 |
| Family-Safe Planner | 5 | 5 | 0.80 | 6 | 3.33 |

### Prioritisation Decision

**Selected feature: Trust-Aware Personalised Trip Assistant**

RICE score: **11.25**

It was selected because it combines itinerary generation with recommendation explanations and trust-aware checks, directly addressing the core problem identified in the assignment.

### Selected Feature Definition

A conversational assistant that collects:
- Destination
- Travel dates or duration
- Budget
- Traveller type
- Interests and preferences

It then creates an itinerary and provides a short explanation for its suggestions.

---

## 7. Research Outcome

The research and prioritisation process identified a product opportunity beyond basic itinerary generation.

The selected direction focuses on helping travellers understand whether an AI-generated plan fits their needs, preferences and budget.

**Next product documentation:** Product requirements, user stories, success metrics, edge cases and scope.

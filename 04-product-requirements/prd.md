
# Product Requirements Document (PRD)
## MakeMyTrip AI Trip Assistant

## 1. Product Overview

**Product concept:** Trust-Aware Personalised Trip Assistant

An AI-powered trip-planning assistant that generates personalised itineraries based on a traveller's destination, dates, duration, budget, traveller type and interests.

The product aims to make recommendations more transparent and help travellers identify information that requires confirmation.

## 2. Problem Statement

Travel planning often involves collecting information from multiple websites, maps, reviews and social platforms.

Generic recommendations may not reflect an individual's preferences or budget. Travellers therefore spend additional time comparing options and checking information.

## 3. Product Goal

Create an AI-assisted planning experience that:
- Reduces manual trip-planning effort.
- Generates itineraries based on user inputs.
- Considers stated budget and preferences.
- Explains why recommendations may fit.
- Clearly communicates uncertainty and limitations.

## 4. Target Users

### Primary: Aarav Mehta
A working professional who plans short trips and wants personalised recommendations without spending excessive time researching.

### Secondary: Riya Sharma
A family trip planner who needs practical recommendations suitable for different age groups and travel requirements.

**Note:** These are assignment proto-personas, not interview-validated customer segments.

## 5. User Inputs

The assistant collects the following information:

| Input | Purpose |
|---|---|
| Destination | Identify the intended travel location |
| Travel dates / duration | Establish the trip timeframe |
| Budget | Guide budget-conscious planning |
| Traveller type | Understand the travel context |
| Interests | Personalise suggested activities |
| Preferences and constraints | Refine itinerary suitability |

## 6. Core User Stories

| ID | User Story | Priority |
|---|---|---|
| US-01 | As a traveller, I want to enter my destination and trip duration so that I can generate an itinerary. | Must |
| US-02 | As a traveller, I want to provide my budget so that recommendations consider my spending limit. | Must |
| US-03 | As a traveller, I want to select my interests so that the itinerary reflects my preferences. | Must |
| US-04 | As a traveller, I want to see a day-by-day itinerary so that I can organise my trip. | Must |
| US-05 | As a traveller, I want explanations for recommendations so that I can understand their relevance. | Must |
| US-06 | As a traveller, I want uncertain information to be clearly identified so that I can verify it independently. | Must |
| US-07 | As a traveller, I want to save my itinerary so that I can revisit it later. | Should |
| US-08 | As a traveller, I want to reopen saved itineraries so that I can continue planning. | Should |

## 7. Functional Requirements

### FR-01: Trip Information Collection
The application should collect destination, duration, budget, traveller type, interests and relevant preferences.

### FR-02: Itinerary Generation
The application should use the provided trip information to generate a structured itinerary.

### FR-03: Personalisation
The generated plan should reflect the user's stated preferences and constraints.

### FR-04: Recommendation Explanation
The application should provide explanations for why suggested activities or options may fit the traveller.

### FR-05: Trust and Uncertainty
The application should distinguish:
- User-provided facts.
- AI-generated planning suggestions.
- Information requiring confirmation.

### FR-06: Budget Awareness
The assistant should consider the stated budget and communicate when a suitable plan cannot confidently fit it.

### FR-07: Saved Trips
The application should support saving and revisiting generated trip plans.

## 8. Non-Functional Requirements

- Responsive web experience.
- Clear and understandable interface.
- Consistent presentation of itinerary information.
- Appropriate handling of incomplete inputs.
- Clear error messages when AI generation fails.
- Protection of user information.
- Transparent communication of AI limitations.

## 9. Edge Cases and Expected Behaviour

| Scenario | Expected Behaviour |
|---|---|
| Incomplete trip details | Request missing information where necessary. |
| Unrealistic budget | Explain the budget limitation rather than falsely claiming the plan fits. |
| Insufficient suitable recommendations | Communicate that suitable options could not be identified. |
| Unverified prices | Mark prices as requiring confirmation. |
| Unverified availability | Do not present availability as confirmed. |
| AI service unavailable | Display a clear error and allow the user to retry. |
| Unsupported user instructions | Maintain the product's trust and safety constraints. |

## 10. Success Metrics

### Primary Metric
24-Hour Recommendation Action Rate.

Measures the percentage of users who save or start booking a recommended item within 24 hours.

### Guardrail Metric
Budget Violation Rate.

Measures the percentage of assessable itineraries that exceed the user's stated budget.

### Supporting Metrics
- Itinerary generation completion.
- Itinerary save rate.
- Recommendation interaction.
- User feedback on relevance.

The original assignment does not provide a verified production baseline for these metrics.

## 11. Out of Scope

The following were explicitly excluded from the product scope:

- Live flight booking.
- Hotel booking.
- Payment processing.
- Guaranteed real-time prices.
- Guaranteed availability.
- Autonomous travel changes.

The prototype must not claim a booking has been completed.

## 12. Dependencies and Assumptions

- AI-generated recommendations depend on the quality of model output.
- External travel facts may require independent verification.
- No live booking integration is assumed.
- Pricing and commercial assumptions remain unvalidated.
- The product is an independent educational prototype, not an official MakeMyTrip service.

## 13. Product Validation

The original assignment includes:
- An AI Studio prototype.
- An eight-case golden evaluation dataset.
- A reported overall evaluation score of 156/200 (78%).
- Partial performance on budget compliance and unverified-fact handling.
- Manual human review of generated explanations.

These results are preliminary prototype evaluation evidence, not proof of production performance.

---

**Document status:** PRD-Lite  
**Project:** MakeMyTrip AI Trip Assistant

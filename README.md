
# MakeMyTrip AI Trip Assistant
### Trust-Aware Personalised Trip Assistant

An AI-powered travel planning product concept focused on personalised itineraries, budget awareness and transparent recommendations.

> An independent educational product management prototype created as part of the AI Product Management programme at iHub DivyaSampark, IIT Roorkee. This is not an official MakeMyTrip product.

---

## Project Documentation

- [Read the Full Product Case Study — Google Docs](https://docs.google.com/document/d/10wBU4fnBjpFu6ONAECIEa7WcDkCtbm5vOI2vWTv-dR0/edit?usp=sharing)
- [View Original Product Management Assignment (PDF)](09-evidence/MakeMyTrip-Product-Assignment.pdf)
- [View Supporting Evidence](09-evidence/)

## 1. Project Overview

Travel planning often involves information scattered across multiple platforms. Travellers need to compare destinations, activities, budgets and recommendations before creating a practical itinerary.

This project explores how an AI-powered assistant can simplify that process by generating itineraries based on individual preferences while making uncertainty and information limitations clear.

**Product vision:** Help travellers plan trips with greater personal relevance, budget awareness and confidence in AI-generated recommendations.

## 2. Product Links

- **[Open AI Prototype](https://ai.studio/apps/57b05f42-d6c8-4c21-8d47-850be9142762)**
- **[View Airtable Product Research and Automation](https://airtable.com/appPtJLboilg3XaVc/shrZtyev2M2jwlcRi)**

## 3. Product Management Process

| Stage | Work Completed |
|---|---|
| Problem Discovery | Defined the travel-planning problem and user needs |
| User Research | Developed proto-personas and competitor analysis |
| Product Strategy | Evaluated opportunities using RICE prioritisation |
| Product Requirements | Created a lightweight PRD and user stories |
| Prototyping | Developed an interactive AI trip-planning prototype |
| AI Evaluation | Tested outputs against an 8-case golden dataset |
| Automation | Connected prototype workflows with Airtable |
| Growth Strategy | Explored monetisation, conversion and growth hypotheses |
| Responsible AI | Defined trust safeguards and human-review practices |

## 4. Key Product Decisions

### Selected Opportunity: Trust-Aware Itinerary Assistant

Four product opportunities were evaluated:

- Smart Itinerary Generator
- Conversational Trip Planner
- Trust-Aware Itinerary Assistant
- Family-Safe Trip Planner

The Trust-Aware Itinerary Assistant received the highest RICE score of **11.25** and was selected for prototyping.

### Core Product Principles

- Personalised itinerary generation.
- Recommendations based on traveller preferences.
- Budget-aware trip planning.
- Clear distinction between user-provided facts and AI suggestions.
- Unverified information labelled as requiring confirmation.

## 5. AI Evaluation Results

The prototype was evaluated using an 8-case golden dataset covering destinations including Jaipur, Goa, Udaipur, Manali, Dubai, Singapore, Bangkok and London.

<details>
<summary>Evaluation summary</summary>

| Metric | Result |
|---|---:|
| Test cases | 8 |
| Total evaluation score | 156/200 |
| Average score | 3.90/5 |
| Overall score | 78% |

**Key findings:**
- Input matching: 8/8 full passes.
- Preference alignment: 8/8 full passes.
- Budget adherence: 0/8 full passes; 8/8 partial passes.
- Unverified-fact handling: 3/8 full passes; 5/8 partial passes.
- Confirmation handling: 8/8 full passes.
- Override resistance: 8/8 full passes.

The evaluation identified budget adherence and information verification as areas requiring improvement.

</details>

**Important limitation:** The evaluation was conducted on a limited prototype dataset. It does not establish production readiness, real-world recommendation accuracy or unbiased performance.

## 6. Automation and Data Workflow

Airtable was used to organise product research and prototype activity.

The research base included:
- Personas
- Opportunity Backlog
- Itinerary Log

The prototype workflow was connected to Airtable to record itinerary activity.

**Automation observations:**
- 8 itineraries were saved in the prototype.
- 6 Airtable itinerary records were created automatically.
- 2 records were added manually after automation failures.
- All 8 outputs were human-reviewed and marked Approved.

This highlighted the importance of monitoring automation reliability rather than assuming every workflow executes successfully.

## 7. Growth and Responsible AI

The project explored:
- A proposed itinerary-sharing growth loop.
- An illustrative acquisition and conversion funnel.
- Subscription pricing hypotheses.
- Responsible AI governance through Govern, Map, Measure and Manage.
- Human review and transparent communication of uncertain information.

Pricing and revenue figures were exploratory assumptions, not validated business results.

## 8. Project Structure

```text
makemytrip-ai-trip-assistant/
│
├── 01-project-overview/
│   └── overview.md
│
├── 02-product-research/
│   └── research.md
│
├── 03-product-strategy/
│   └── product-strategy.md
│
├── 04-product-requirements/
│   └── prd.md
│
├── 05-prototype/
│   └── prototype-and-user-flow.md
│
├── 06-ai-evaluation/
│   └── ai-evaluation.md
│
├── 07-automation/
│   └── airtable-automation.md
│
├── 08-growth-and-responsible-ai/
│   └── growth-and-responsible-ai.md
│
├── 09-evidence/
│   ├── README.md
│   ├── MakeMyTrip-Product-Assignment.pdf
│   ├── prototype-home.png
│   ├── generated-itinerary.png
│   └── saved-itinerary.png
│
└── README.md
```

## 9. Supporting Evidence

See the [`09-evidence`](09-evidence/) folder for the original assignment and selected prototype screenshots.

## 10. Limitations and Next Steps

This project is an educational prototype, not a production travel platform.

The work did not include:
- Live travel booking or payment integration.
- Guaranteed real-time prices or availability.
- Validation through real customer interviews.
- Production deployment or revenue testing.
- Automated bias detection or automatic system-pause mechanisms.

**Potential next steps:**
1. Conduct user interviews and usability testing.
2. Improve budget adherence and itinerary consistency.
3. Strengthen verification of travel information.
4. Measure real user engagement and conversion.
5. Test pricing and growth hypotheses.

---

## Project Information

**Project:** MakeMyTrip AI Trip Assistant  
**Category:** AI Product Management  
**Programme Context:** iHub DivyaSampark, IIT Roorkee  
**Tools:** Google AI Studio, Airtable  
**Project Type:** Independent educational prototype

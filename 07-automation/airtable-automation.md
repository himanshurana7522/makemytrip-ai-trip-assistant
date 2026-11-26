
# Airtable Automation Documentation

## 1. Overview

Airtable was used as the supporting data and automation layer for the MakeMyTrip AI Trip Assistant product prototype.

The Airtable base is named:

**MakeMyTrip AI Trip Assistant — Product Research**

It was designed to organise product research, connect personas with product opportunities, and maintain records of generated itineraries, AI explanations and human review status.

**Open the Airtable Base:**  
https://airtable.com/appPtJLboilg3XaVc/shrZtyev2M2jwlcRi

## 2. Airtable Database Structure

The Airtable base contains three tables.

### A. Personas

**Purpose:** Store the project personas and their key characteristics.

Key fields:
- Persona Name
- Segment Tags
- Top Latent Need
- Top Pain Point
- Top Goal

The table includes:
- Aarav Mehta — Primary Persona
- Riya Sharma — Secondary Persona

### B. Opportunity_Backlog

**Purpose:** Store and prioritise product opportunities.

Key fields:
- Idea
- Reach
- Impact
- Confidence
- Effort
- RICE Score
- Decision
- Target Persona

The Target Persona field is configured as a linked record to the Personas table.

### C. Itinerary_Log

**Purpose:** Maintain records of generated travel itineraries and their AI explanations.

Key fields:
- Timestamp
- Persona
- Itinerary Summary
- AI Explanation
- Review Status

The Persona field is configured as a linked record to the Personas table.

## 3. Automation Workflow

The intended workflow was:

1. A user generates an itinerary in the AI Trip Assistant.
2. The itinerary is saved in the application.
3. A corresponding record is created in Airtable's Itinerary_Log table.
4. An AI Explanation is generated after the configured trigger conditions are met.
5. The explanation is reviewed by a human.
6. The record receives its final review status.

## 4. Eight-Scenario Automation Test

Eight golden-dataset itineraries were used to test the workflow.

| Test | Destination | Record Creation |
|---|---|---|
| G1 | Jaipur | Automatic |
| G2 | Goa | Automatic |
| G3 | Udaipur | Automatic |
| G4 | Manali | Manual |
| G5 | Dubai | Automatic |
| G6 | Singapore | Automatic |
| G7 | Bangkok | Automatic |
| G8 | London | Manual |

### Automation Results

- 8 itineraries were saved in the application.
- 6 Airtable records were created automatically.
- 2 records (Manali and London) required manual creation.
- AI explanations were generated after the applicable trigger conditions were met.
- All 8 records were reviewed by a human and marked Approved.

**Automatic record creation success: 6/8 scenarios (75%).**

## 5. Human Review Process

Human review was retained as an important part of the workflow.

All eight records were reviewed and marked Approved after human review.

The automation did not independently establish that every recommendation was accurate, current or unbiased.

## 6. Limitations and Learnings

The testing identified the following limitations:

- Automatic Airtable record creation was not reliable in all eight scenarios.
- Manali and London required manual record creation.
- Human review was required before approval.
- The workflow did not automatically detect recommendation bias.
- The workflow did not automatically pause recommendations when a risk was identified.

### Improvement Opportunities

1. Improve application-to-Airtable record creation reliability.
2. Add error handling and retry logic for failed records.
3. Maintain clear review states for pending and approved records.
4. Improve traceability between saved itineraries and Airtable records.
5. Retain human review for important trust and safety decisions.

## 7. Project Outcome

The Airtable workflow demonstrated how itinerary records, AI-generated explanations and human review could be organised in a structured process.

Six of eight records were created automatically, while two required manual intervention.

This was a prototype-level workflow, not a fully reliable production automation system.

## 8. Project Resource

**Airtable Product Research Base:**  
https://airtable.com/appPtJLboilg3XaVc/shrZtyev2M2jwlcRi

The Airtable base provides supporting evidence of the product research structure and itinerary logging used in this project.


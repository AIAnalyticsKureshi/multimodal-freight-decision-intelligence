# Multimodal Freight Decision Intelligence Dashboard (Germany)

## Overview

This project presents an interactive Power BI dashboard designed to support freight transport decisions across Germany. It evaluates three transport modes — **Road, Rail, and Inland Waterway (IWT)** — against the three performance dimensions that matter most in practice:

- **Cost**
- **Transit Time**
- **CO₂ Emissions**

The goal of the project is not simply to visualize logistics data, but to convert transport performance into a **decision-support system**. The dashboard helps users compare modes, understand trade-offs, test scenario impacts, and identify the most appropriate transport choice under different operational conditions.

---

## Business Problem

In freight planning, choosing a transport mode is rarely straightforward. The cheapest mode may not be the fastest. The fastest option may not be the most sustainable. A greener alternative may introduce both time and cost penalties.

This creates a recurring business problem:

> How can logistics managers and supply chain decision-makers choose the most appropriate transport mode when cost, speed, and emissions often conflict?

This dashboard addresses that problem by structuring mode comparison into a clear decision framework.

---

## Project Objective

The objective of this project is to build a **multilayer decision-intelligence dashboard** for multimodal freight transport in Germany that allows users to:

- compare Road, Rail, and Inland Waterway across key KPIs
- evaluate cost–CO₂–time trade-offs
- assess the effect of different scenarios
- derive a final mode recommendation in a structured, transparent way

---

## Dashboard Structure

The dashboard is built as a **single interactive page** with button-based navigation between four analytical layers.

### 1. Overview
The Overview layer provides a high-level comparison of all transport modes for the selected corridor and scenario.

It highlights:
- Shipment Cost (€)
- Transit Time (h)
- CO₂ Intensity (g/tkm)
- Shipment CO₂ (kg)

This layer answers:
- Which mode is cheapest?
- Which mode is fastest?
- Which mode is cleanest?

---

### 2. Trade-Off Intelligence
The Trade-Off Intelligence layer focuses on the decision cost of switching between modes.

It highlights:
- **Extra Cost vs Cheapest**
- **CO₂ Reduction vs Highest**
- **Time Penalty vs Fastest**

This layer translates raw metrics into real business trade-offs and answers:
- How much more does a cleaner option cost?
- How much delay does a greener option create?
- Is the switch operationally and financially justified?

---

### 3. Scenario Analysis
The Scenario Analysis layer evaluates how performance changes under different operating conditions.

Scenarios include:
- Baseline / Current Conditions
- Fuel Cost Shock
- High Carbon Price
- Express Rail Improvement

This layer answers:
- How sensitive are mode choices to external changes?
- Which scenarios improve or weaken the competitiveness of each mode?
- How do policy and operating changes affect cost, emissions, and time?

---

### 4. Decision Intelligence
The Decision Intelligence layer consolidates the full analysis into a final recommendation.

It highlights:
- Recommended Mode
- Recommended Cost
- Recommended CO₂
- Recommended Transit Time

This layer answers:
- Which mode is the most balanced option under the selected corridor and scenario?
- How do the alternatives compare against the recommended choice?

---

## Analytical Approach

The dashboard is designed as a **decision-support product**, not just a reporting interface.

The analytical logic combines:

- **absolute performance metrics**  
  (cost, emissions, transit time)

- **relative trade-off metrics**  
  (extra cost, time penalty, CO₂ reduction)

- **scenario sensitivity logic**  
  (how results shift under different assumptions)

- **decision intelligence**  
  (final recommendation based on comparative performance)

This structure makes the dashboard useful not only for descriptive analysis, but also for practical logistics evaluation.

---

## Key Performance Indicators

The dashboard uses the following core KPIs:

- **Total Cost (€) - Fixed 24t**
- **Transit Time (h)**
- **WTW CO₂ Intensity (g/tkm)**
- **Total WTW CO₂ (kg) - Fixed 24t**
- **Extra Cost vs Cheapest (€)**
- **CO₂ Reduction vs Highest (%)**
- **Time Penalty (h)**

These KPIs allow both **absolute comparison** and **decision-focused interpretation**.

---

## Main Insights

The dashboard consistently shows the structural differences between the three transport modes:

- **Road** is generally the fastest mode, but also the most emission-intensive.
- **Rail** typically offers the best environmental performance and often emerges as the strongest balanced option.
- **Inland Waterway** is often the lowest-cost mode, but comes with a substantial transit-time penalty.

This confirms that multimodal freight decisions are not about finding a universally “best” mode, but about identifying the best fit under specific business priorities.

---

## Tools Used

- **Power BI** — dashboard design, data modeling, DAX measures, bookmarks, interactive navigation
- **Excel** — data preparation and structuring
- **DAX** — KPI logic, trade-off measures, scenario measures, recommendation logic

---

## Technical Highlights

This project includes:

- a **single-page interactive dashboard architecture**
- **bookmark-based navigation** across four analytical layers
- mode-level and scenario-level KPI comparison
- trade-off intelligence built around cost, emissions, and time
- a final **decision recommendation layer**

---

## Why This Project Matters

This project demonstrates how business intelligence can be applied to a real logistics problem where multiple objectives conflict.

Instead of treating cost, time, and emissions as separate metrics, the dashboard integrates them into a single decision framework. This makes the output more useful for:

- logistics managers
- supply chain analysts
- sustainability-oriented transport planning
- business intelligence and reporting roles

---

## Files in This Repository

```text
dashboard/   → Power BI dashboard file (.pbix)
data/        → cleaned dataset (.xlsx)
images/      → dashboard screenshots
docs/        → supporting project documentation
README.md    → project overview

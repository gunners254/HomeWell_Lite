# HomeWell Lite – Damp & Mould Risk Decision-Support Prototype

🚧 Prototype — built to explore decision-support for housing operations, not production deployment

## What this is

HomeWell Lite is an explainable analytics prototype designed to support **damp and mould inspection triage in social housing**.

It demonstrates how data can be used to:

* prioritise inspections
* identify higher-risk properties
* support earlier intervention decisions

## Key insight

The modelling shows a clear operational reality:

* Reactive, complaint-linked triage performs best
* Future risk prediction is weaker but still useful as an exploratory signal
* Pre-complaint prediction is not currently strong enough for operational use

This reflects real-world data limitations rather than model choice.

## Operational Positioning

This prototype is best used as a **decision-support layer**, not a standalone system.

It should sit upstream of:

* inspection scheduling
* case review
* housing officer decision-making

It is designed to support:

* prioritisation of limited inspection capacity
* triage of incoming complaints
* early identification of potential escalation

It should not be used as:

* a final decision engine
* a replacement for case-level judgement



## Overview

HomeWell Lite is a predictive analytics prototype designed to support early identification of damp and mould risks in social housing.

The goal is to move from reactive complaint handling to proactive risk-based intervention.

## Problem

Social housing providers often respond to damp and mould issues only after tenant complaints.

This reactive approach:

* Increases repair costs
* Impacts tenant health
* Creates regulatory and reputational risk

## Approach

This prototype uses machine learning models to:

* Predict future damp/mould risk scores for properties
* Prioritise inspections based on risk
* Provide explainability for decision-making

## Key Features

* Reactive Risk Triage (current cases)
* Future Risk Prediction (proactive identification)
* Explainable outputs (feature importance/drivers)
* Simple dashboard interface (Streamlit)

## Demo Screenshots

### Reactive Triage
![Reactive Triage](./Reactivetriage.jpeg)

### Future Damp Risk
![Future Risk](./Futurerisk.jpeg)

### Escalation Prioritisation
![Escalation](./Escalationprioritisation.jpeg)

### Model Limitations
![Limitations](./Modellimitations.jpeg)


## Tech Stack

* Python
* Scikit-learn
* Pandas / NumPy
* Streamlit

## Why model performance varies

The three modelling modes highlight a key structural challenge:

* Reactive triage performs best because complaint signals are strong and immediate
* Future damp risk is harder because it relies on weaker proxy signals (EPC + early behaviour)
* Pre-complaint prediction is weakest due to the lack of early indicators

This is not a modelling issue — it is a **data generation problem**.

Stronger proactive performance would require:

* environmental data (humidity, temperature)
* repair history
* property condition surveys
* tenant vulnerability indicators


## Limitations

* Synthetic/limited dataset
* Not production-hardened
* No real-time data integration

## Positioning

This is not a full housing management system.

It is a **decision-support layer** designed to sit upstream of inspections, repairs, and capital planning.

## Author

Victor Adewale Adesope
Founder, Stratise AI Labs Ltd

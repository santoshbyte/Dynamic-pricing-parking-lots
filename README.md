#  Dynamic Pricing for Urban Parking Lots
Dynamic pricing model for urban parking lots using real-time data and intelligent feature engineering — built during Summer Analytics 2025.

## Project Overview
This project aims to implement a dynamic pricing system for urban parking lots based on real-time data such as occupancy, traffic, vehicle type, and queue length using the Pathway streaming engine.

dynamic-parking-pricing/
│
├── data/
│   └── cleaned.csv
│
├── notebooks/
│   └── dynamic_pricing_pipeline.ipynb
│
├── src/
│   └── pricing_model.py
│
├── architecture.md or architecture.png
├── README.md
├── requirements.txt
└── LICENSE (optional)

## Tech Stack
-  Python
-  [Pathway](https://pathway.com/)
-  Pandas for preprocessing
-  Mermaid for architecture diagram
-  Git & GitHub

## Architecture Diagram
```mermaid
flowchart TD
    A[Input CSV: Parking Data] --> B[Preprocessing using Pandas]
    B --> C[Pathway Schema + UDFs]
    C --> D[Feature Engineering]
    D --> E[Dynamic Pricing Model]
    E --> F[Stream Output JSONL]


#Emergency Resource Dispatch Analyzer

Problem Overview
----------------
This project analyzes emergency resource requests reported by different zones during a disaster drill. Each request is categorized into Low, Moderate, High, or Invalid demand using conditional logic. After classification, a personalized filtering rule is applied to modify the final dispatch plan.
The program ensures structured data processing using lists, loops, and conditional statements without using advanced built-in functions.

Features
--------
Accepts multiple resource request values as input
Categorizes requests into:
Low Demand (1–20)
Moderate Demand (21–50)
High Demand (>50)
Invalid Requests (<0)
Counts total valid requests (≥ 0)
Applies personalized filtering using PLI
Generates a final dispatch report

Logic / Approach Used
---------------------
The program first takes the number of requests and stores them in a list using a loop.
Each value is processed using conditional statements:
Negative values → Invalid
Zero → Valid (No Demand)
1–20 → Low Demand
21–50 → Moderate Demand
50 → High Demand
Valid requests are counted during classification.
A Personalized Logic Index (PLI) is calculated.
Based on PLI, one demand category is removed.
The final filtered lists and summary are displayed.

Personalization Applied
-----------------------
Last 5 digits of Registration Number = ________
Personalized Logic Index (PLI) = L % 3
Filtering Rules:
PLI = 0 → Remove Low Demand
PLI = 1 → Remove Moderate Demand
PLI = 2 → Remove High Demand
This ensures unique dispatch behavior for different students based on their registration number.

Repository Structure
-------------------
Emergency-Resource-Dispatch-Analyzer/
│
├── challenge5.py
├── README.md
└── test_cases.txt

Language
--------
Python

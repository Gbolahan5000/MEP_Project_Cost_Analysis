# MEP Project Operations Analyst Simulation

## Your role
You have just joined **Apex MEP Services Ltd.** as a Project Operations Analyst.

The company delivers mechanical, electrical and plumbing services across commercial, residential,
healthcare, hospitality, industrial, retail and technology projects in Nigeria.

You report to the Head of Operations. You have been given an export of the company's operational
data and asked to make sense of it before the next management review.

## The stakeholder request

> "We have several projects running at the same time. Some appear to be profitable, while others
> are experiencing delays, labour overruns, procurement issues and slow collections. I don't want
> another dashboard full of numbers. I need you to tell me what is actually happening across the
> portfolio, what is driving it, where management should pay attention, and what actions we should
> consider."

## Your assignment

Treat this like your first 2-3 weeks on the job.

You are NOT expected to start by building a dashboard.

Your work should move through these stages:

1. **Understand the business**
   - What does an MEP contractor do?
   - How does a project make or lose money?
   - What operational levers can management actually influence?

2. **Profile the data**
   - Identify the grain of every table.
   - Check missing values, duplicates, date problems and suspicious records.
   - Identify relationships between tables.
   - Decide which data can safely be joined and at what grain.

3. **Build a business view**
   Investigate project performance using measures such as:
   - Contract value
   - Approved budget
   - Actual labour cost
   - Actual material cost
   - Cost variance
   - Project margin / estimated margin
   - Labour-hour variance
   - Schedule variance
   - Change-order value
   - Outstanding receivables
   - Procurement delays

4. **Diagnose, don't just describe**
   If you find that costs are above budget, investigate:
   - Which projects?
   - Which disciplines?
   - Which work categories?
   - Which suppliers/materials?
   - Which project types?
   - Are overruns linked to delays, rework, procurement or scope changes?

5. **Produce management findings**
   Your final output should contain a small number of high-confidence findings.
   Each finding should state:
   - What happened
   - Magnitude
   - Where it is concentrated
   - Likely operational driver(s)
   - Business implication

6. **Recommend actions**
   Recommendations must be specific enough for a manager to act on.
   Include a suggested owner and a metric that could be monitored afterwards.

## Important constraint

Do not assume every problem requires a dashboard.

Use the tool that fits the question:
- Excel for ad-hoc analysis, reconciliation and financial modelling
- SQL for extracting and joining operational data
- Power BI for recurring monitoring
- Python only if it materially improves the analysis

Your portfolio project should demonstrate **analytical judgement**, not the number of tools used.

## Suggested final deliverables

### A. Analytical workbook
A clean Excel workbook containing your calculations, checks and supporting analysis.

### B. SQL analysis
A `.sql` file containing your main analytical queries.

### C. Management briefing
A 5-7 slide PowerPoint or 2-3 page written management memo answering:
1. What is happening?
2. What is driving it?
3. Which areas deserve management attention?
4. What should management consider doing?
5. How should the business monitor whether the actions work?

### D. Optional dashboard
Build this only if you conclude that recurring operational monitoring would benefit from one.

## Rules for the simulation

- Do not search for the hidden answer.
- Do not assume the data is clean.
- Do not manufacture explanations that the data cannot support.
- Separate correlation from causation.
- State assumptions.
- Quantify important claims.
- If two tables cannot safely be joined, explain why.
- If the data is insufficient to answer a question, say so.
- Your job is not to make the company look good or bad. Your job is to make the situation understandable.

## Dataset structure

01_Projects.csv
- One row per project.

02_Work_Orders.csv
- One row per project work package/order.

03_Labour_Entries.csv
- Time/cost entries recorded against work orders.

04_Procurement.csv
- Purchase orders and supplier delivery performance.

05_Suppliers.csv
- Supplier reference data.

06_Change_Orders.csv
- Project scope changes and their schedule/value impact.

07_Invoices.csv
- Project billing and collection information.

08_Milestones.csv
- Planned vs actual project milestones.

09_Issues_Log.csv
- Operational issues recorded during projects.

10_Employees.csv
- Employee reference data.

11_Clients.csv
- Client reference data.

## Data-quality note

There are intentional data-quality issues in the files.

Do not "fix" them silently. Identify them, document them and decide how they affect the analysis.

## Portfolio positioning

When finished, this should not be presented as:

"MEP Power BI Dashboard."

Present it as something closer to:

**MEP Project Operations Analysis**
*Project Operations Analyst Simulation*

Business problem → data investigation → diagnosis → operational implications → recommendations.
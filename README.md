# Data Bank System (ERD) for Provincial Government of Bataan

A real-world enterprise analytical data repository designed and built for the **Provincial Government of Bataan**, centralizing performance measurements across **37+ departments and offices**. The system tracks the **Governor's Joint Strategic Goals (GJSG)** priority indicators — reducing data fragmentation, eliminating redundant data requests, and promoting transparency and accountability across regional governance.

View the Entity-Relationship Diagram [here](https://dbdiagram.io/d/Initial_ERD_for_Data_Bank_System-2-69854dc7bd82f5fce2d4deb8)

---

## Project Overview

The Provincial Government of Bataan manages 37+ departments that each track their own KPIs independently — leading to fragmented data, redundant reporting, and slow decision-making. This data bank system solves that by providing a unified, centralized analytical repository that connects all departments under one structured data model.

**Key outcomes the system addresses:**
- Eliminates data silos and fragmentation across departments
- Reduces time-consuming manual coordination and redundant data requests
- Improves inefficient service delivery through structured data governance
- Promotes transparency and accountability at the provincial level

---

## Tech Stack
- **Data Modeling:** DBML · dbdiagram.io
- **Schema Design:** Galaxy Schema · Dimensional Modeling · 3NF Normalization
- **Database:** PostgreSQL
- **Concepts:** Data Catalog · Data Lineage · Data Observability · ETL/ELT

---

## Architecture

The system is built on a **Galaxy Schema** — a multi-fact table dimensional model with shared dimensions across departments. This allows cross-departmental querying and reporting without data duplication.

### Core Data Engineering Components

**Data Observability**
Structured logging and metrics tracking across the entire pipeline — recording submission dates, update timestamps, responsible entities, job success/failure events, and source data traceability.

**Data Lineage**
Full lineage tracking across every dataset — documenting what data was extracted, transformed, and loaded, when it happened, where it came from, and how it was processed.

**Data Catalog**
A comprehensive governance layer covering:
- Metadata and search/discovery features
- Departmental data agreements and measurement methodology
- Submission schedules, reporting cut-off dates, and escalation procedures
- Access controls, data privacy policies, and role responsibilities
- Integration connections to actual department data sources

**Data Orchestration**
Pipeline automation design supporting batch scheduling, near real-time, and real-time data ingestion across departments.

---

## Scope — Indicators Tracked

39 priority indicators across departments including infrastructure, healthcare, education, governance, tourism, economic development, and public safety.

| Lead Department | Indicator | Status |
|---|---|---|
| OPPDC | % increase in barangays with completed Barangay Master Development Plans | Done |
| OPPDC | % reduction in inflation rates through price monitoring | Done |
| Legal & PHRMO | % increase in citizen concerns addressed via 8888 hotline | Done |
| PHRMO | % improvement in government employee service quality | Done |
| MBDA | % reduction in crime rates through law enforcement collaboration | Done |
| MBDA, PNP, PDRRMO | % reductions in accidents by place of occurrence | Done |
| MBDA & PDRRMO | % reduction of injury among affected population during calamity | Done |
| PIO | % improvement in government service delivery via social media | Done |
| PITO | % increase in implementation of digital governance systems | Done |
| PGO | % improvement in citizen access to services | Done |
| PGO | % of LGUs enrolled in Performance Governance System (PGS) | Done |
| PGO | % increase in innovation hubs established | Done |
| PGO | % growth in defense industry investments | Done |
| PGO | % increase in renewable energy projects and green mobility adoption | Done |
| PGO | % increase in community participation in fitness programs | Done |
| PGO | % improvement in school health programs | Done |
| PGO | % reduction in youth smoking and vaping rates | Done |
| PGO | % increase in participation in sports programs | Done |
| PGO-INB | % increase in scholarship recipients and licensure exam pass rates | Done |
| PGO | % increase in teacher capacity building and use of LMS | Done |
| PGO | % integration of values education in school curricula | Done |
| PGO | % reduction in out-of-school youth through skills and employment programs | Done |
| PGO | % increase in family engagement in children's education (Educhild Campaign) | Done |
| PGO-BHSS | % improvement in school health and wellness programs | Done |
| PGO | % increase in adult literacy and lifelong learning participation | Done |
| PGSO-PMO | % improvement in management and efficiency of public enterprises | Done |
| PEO | % increase in disaster-resilient infrastructure | Done |
| PEO | % improvement in infrastructure and market access | Done |
| PEO | % increase in access to healthcare facilities | Done |
| PEO | % increase in access to clean water and sanitation facilities | Done |
| PEO | % increase in school infrastructure development | Done |
| PPPIC | % increase in locators in FAB Expansion Areas | Done |
| PPPIC | % increase in public-private partnerships (PPPs) | Done |
| LFC | % increase in government revenue | Done |
| PCEDO | % increase in SMEs using online systems for business permits | Done |
| PCEDO | % adoption of electric vehicles in public transport | Done |
| PCEDO | % increase in TNVS slots for public transport | Done |
| PTourism | % increase in tourism activities and festival revenue | Done |
| PTourism | % increase in compliance with ecological and tourism fees | In Progress |

---

## Key Design Decisions
- **Galaxy Schema** chosen over star schema to support shared dimensions across multiple fact tables — enabling cross-departmental analytics without redundancy
- **3NF Normalization** applied to all dimension tables to ensure 100% referential integrity
- **Full data catalog** designed before implementation to establish clear governance agreements with each department
- **Audit tables** planned to reference all facts and dimensions with submission and verification tracking

---

## What I Learned

Designing a data system for a real government client with 37+ stakeholders taught me that data engineering is as much about people and governance as it is about technology. Aligning departments on definitions, submission schedules, and data ownership was as complex as the schema design itself.

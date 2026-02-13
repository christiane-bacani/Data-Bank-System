# Data Bank System for Provincial Government of Bataan

An analytical data repository for the Provincial Government of Bataan that centralizes performance measurements across 37+ departments and/or offices. Built to track the **Governor's Joint Strategic Goals (GJSG)** priority indicators, this data repository reduces time-consuming coordination, redundant data request, improves inefficient service delivery, removes data fragmentation and silos, and promotes transparency and accountability.

## Table of contents
- [Undercurrent of the Data Bank](#Undercurrent-of-the-Data-Bank)
- [Todo](#Todo)
- [Status Table](#Status-Table)

## Undercurrent of the Data Bank

### Data Observability
- Using logging, metrics, and tracking such as lineage.

### Logging
- Use to record events such as the date when the data is submitted, date when the data is updated, name of the entity who submitted the data, name of the entity who updated the data, specific job/module/class/function that has an error, specific job/module/class/function that is successful, date of when the job/module/class/function is successful, date when the job/module/class/function cause error, source data that causes error, source data that was successful, etc.

### Data Lineage
- Tracker to track what/when/where/how the data was extracted, transformed, and loaded.

### Data Orchestration/Queuing
- Tools to automate the pipeline by batch scheduling, near real-time, and/or real-time.

### Data Catalog
- Contains all the necessary utilities of the pipeline such as the data lineage, metadata, search and discovery features to get the data they needed, agreements for the data/indicators/success indicators to be used per department and make sure it was clear on how do you track it and considered it as a failure and documented in the methodology, agreements on how to measure the indicators/success indicators, agreements on how to submit the data, agreements on who is/are the people who will submit the data, agreements on systems to use (if feasible) that sends that data or supports the extraction of the data, agreements on what date/time/period they needed to submit the data, agreements on how much time period is valid before the data bank perform automated escalation, agreements on proper escalation process if they don't send the data on time, information about who can access the different datasets on the data bank, feedback data of the users of the data bank, integration connections (links to the actual data source of the dataset).

## Todo
- Create the star schema of the pending status
- Check every facts table which facts table has shared dimension and create shared dimension based on that facts table

## Status Table

| Lead Department | Indicator | Status|
|-----------------|-----------|-------|
|   OPPDC         | % increase in barangays with completed Barangay Master Development Plans | Done |
|   OPPDC         | % reduction in inflation rates through price monitoring and direct selling of basic commodities | Done |
| Legal & PHRMO   | % increase in citizen concerns addressed via the 8888 hotline | Done |
| PHRMO           | % improvement in government employee service quality | Done |
| MBDA            | % reduction in crime rates through collaboration with law enforcement | Done|
| MBDA, PNP, and PDRRMO | % reductions on accidents (place of occurrence) | Done |
| MBDA and PDRMOO | % reduction of injury among affected population during calamity | Done |
| PIO             | % improvement in government service delivery via social media | Done |
| PITO            | % increase in implementation of digital governance systems | Done |
| PGO             | % improvement in citizen access to services | Done |
| PGO             | % of LGUs enrolled in the Performance Governance System (PGS) with performance-based incentives | Done |
| PGO             | % increase in innovation hubs established | Pending | 
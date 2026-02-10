# Data Bank System for Provincial Government of Bataan

An analytical data repository for the Provincial Government of Bataan that centralizes performance measurements across 37+ departments and/or offices. Built to track the **Governor's Joint Strategic Goals (GJSG)** priority indicators, this data repository reduces time-consuming coordination, redundant data request, improves inefficient service delivery, removes data fragmentation and silos, and promotes transparency and accountability.

## Table of contents
- [Todo](#Todo)
- [Status](#Status)
- [Undercurrent of the Data Bank](#Undercurrent-of-the-Data-Bank)

## Todo
- Create the data model for measuring the indicators for reduction pct of injuries/casualties during calamities

## Status
- % increase in barangays with completed Barangay Master Development Plans (OPPDC) - `DONE`
- % reduction in inflation rates through price monitoring and direct selling of basic commodities (OPPDC) - `Done`

<br>

- % increase in citizen concerns addressed via the 8888 hotline (Legal & PHRMO) - `DONE`
- % improvement in government employee service quality (PHRMO) - `DONE`

<br>

- % reduction in crime rates through collaboration with law enforcement (MBDA) - `DONE`
- % reductions on accidents (place of occurrence) (MBDA, PNP, and PDRRMO) - `DONE`
- % reduction of injury among affected population during calamity (MBDA, PDRRMO) - `PENDING`

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
- Contains all the necessary utilities of the pipeline such as the data lineage, metadata, search and discovery features to get the data they needed, papers/agreements for the indicators used for every fact table and data to be use, papers/agreements if they don't send the data on time or proper process if they don't send the data on the given agreement, info about who can view/use different datasets, feedback about the datasets, integration connections (links to the actual data source of the dataset).
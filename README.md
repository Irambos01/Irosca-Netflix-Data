# Project 3: Netflix Dataset Movies and TV shows Records.

# 1. Executive Summary

This project provides a comprehensive data auditing, cleaning, and exploratory data analysis (EDA) pipeline for Netflix's global title catalog (up through late 2020). Operating on a dataset of 7,789 initial records, the primary goal was to inspect data hygiene, eradicate duplicates, quantify missingness across metadata fields, and establish a foundational structure for downstream visual analytics and content strategy research.

# 2. Business & Analytical Objectives

Data Quality Audit: Evaluate data types, structural anomalies, and integrity constraints across all catalog attributes.

Deduplication: Locate and remove exact and near-duplicate title entries to prevent skewed metric aggregations.

Missingness Diagnostics: Identify pattern-level missing data across critical fields (e.g., Director, Cast, Country) and understand underlying causes (e.g., TV series vs. standalone movies).

Data Standardization: Prepare clean data schemas for statistical profiling, time-series analysis, and demographic tag breakdown.

# 3. Data Profile & Architecture

Raw Row Count: 7,789 rows

Post-Cleaning Row Count: 7,787 rows (2 redundant entries removed)

Feature Attributes: 11 attributes covering identifiers, classification, production details, and release metrics.

# 4. Key Findings & Data Hygiene Highlights

Redundancy Elimination:

Identified and purged 2 duplicate records (Show_Id: s684 - Backfire and Show_Id: s6621 - The Lost Okoroshi).

Structural Missingness Patterns:

The high rate of missing directors (~30.7%) is structurally expected due to the distinction between episodic TV Shows (often managed by showrunners rather than single directors) and feature films.

Core Reliability:

Essential metadata attributes (runtime duration, category, genres) are 100% complete, providing a solid baseline for content distribution and duration analyses.

# 5. Technical Stack

Language: Python 3.x

Data Manipulation: pandas, numpy

Data Visualization: seaborn, matplotlib

Environment: Jupyter Notebook

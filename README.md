# Hospital OPD Analytics Pipeline

SQL-based analytics pipeline for a ~1M+ record HOSxP hospital system (patient: 40K+, ovst: 500K+).

## Impact
- Enabled analytics across ~1M+ legacy hospital records  
- Improved query performance via simplified multi-table joins  
- Supported outpatient, billing, and clinical reporting workflows  

## Overview
SQL-first pipeline for transforming and analyzing highly normalized, undocumented hospital data from legacy HOSxP systems.

## Architecture
HOSxP (MySQL) → SQL ETL Layer → Analytics Views → Reports / Dashboards

## Tech Stack
- MySQL  
- SQL (ETL / Analytics)  
- HOSxP Hospital System  

## Data Model (OPD)
- patient — demographics  
- ovst — outpatient visits  
- opdscreen — screening data  
- vn_stat — visit-level financial summary  
- opitemrece — billing line items  
- drugitems — drug catalog  
- nondrugitems — non-drug services  
- pttype / pttypeno — insurance / coverage  
- spclty / kskdepartment / clinic — organization structure  
- doctor / opduser — staff  
- icd101 — ICD-10 codes  
- icd9cm1 — ICD-9 codes  
- lab_head / lab_order — laboratory data  
- oapp — appointments  
- thaiaddress — address hierarchy

#Part-1-Occupancy-Reconciliation

# Residential Portfolio Operations/Part 1: Occupancy Reconciliation

[Project4_Part1_Occupancy_Reconciliation.xlsx](https://github.com/user-attachments/files/31519782/Project4_Part1_Occupancy_Reconciliation.xlsx)

## Project Overview

This is the first part of my **Residential Portfolio Operations** project.

I reviewed occupancy data across a **Property Register** and **Active Tenancies** dataset to check whether property occupancy statuses were consistent between the two sources.

The aim was to identify record-level discrepancies that could affect portfolio reporting and operational decisions.

---

## Key Skills Demonstrated

### Record-Level Data Reconciliation

I used `PropertyID` as the common key to match records between the Property Register and Active Tenancies.

Using **XLOOKUP**, I retrieved tenancy information for each property and derived an occupancy status based on whether an active tenancy was found.

I then compared this result with the existing `RegisterStatus` using an **IF formula** to flag records as either `Match` or `Mismatch`.

![01_Record_Level_Occupancy_Reconciliation]("https://github.com/user-attachments/assets/fc8fd300-a2f7-4442-ad47-6da16cd7bda0")


*Record-level occupancy reconciliation showing matched records and highlighted mismatches.*

### Exception Identification

The cross-check identified **2 occupancy mismatches from 20 properties**:

* one property recorded as **Occupied** in the Property Register but with no matching active tenancy;
* one property recorded as **Void** despite having an active tenancy.

This resulted in a **90% match rate**.

Conditional formatting was used to make exceptions immediately visible for investigation.

### Pivot Table Summary

I created a Pivot Table to summarise reconciliation results by borough.

The summary showed:

* **18 matched records**
* **2 mismatches**
* mismatches identified in **Ealing** and **Hounslow**

![02_Occupancy_Reconciliation_By_Borough]("https://github.com/user-attachments/assets/65f6318f-259c-4f22-8ab6-ae8f0a31edf2")

*Occupancy reconciliation summary by borough.*

A useful finding from this exercise was that portfolio-level totals can appear reasonable while individual property records still contain inconsistencies. This is why record-level reconciliation is important before relying on aggregated reporting.

---

## Tools Used

* Microsoft Excel
* XLOOKUP
* IF
* COUNTIF
* Conditional Formatting
* Pivot Tables
* Excel Tables and structured references

---

## Outcome

The review created a clear occupancy reconciliation process that:

* matches property and tenancy records using a common key;
* derives occupancy status from active tenancy data;
* identifies mismatches requiring investigation;
* summarises exceptions at portfolio and borough level.

This provides a more reliable basis for occupancy reporting and portfolio management decisions.

---

## Next Part

**Part 2 — Rent & Arrears Performance**

The next stage will review rent charged, rent received, arrears and collection performance across the same residential portfolio.




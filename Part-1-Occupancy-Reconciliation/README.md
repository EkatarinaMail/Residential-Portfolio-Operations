# Residential Portfolio Operations

## Part 1: Occupancy Reconciliation

## Project Overview

I compared the **Property Register** with **Active Tenancies** to check whether occupancy statuses matched at property level.

The aim was to identify discrepancies before using the data for portfolio reporting.

---

## Key Skills Demonstrated

### Occupancy Reconciliation

I used `PropertyID` as the common key and **XLOOKUP** to match tenancy records to properties.

I then used an **IF formula** to compare `RegisterStatus` with the occupancy status derived from active tenancy data.

![01\_Record\_Level\_Occupancy\_Reconciliation](https://github.com/user-attachments/assets/fc8fd300-a2f7-4442-ad47-6da16cd7bda0)

*Record-level reconciliation with mismatches highlighted.*

### Exception Review

The cross-check identified:

* **20 properties reviewed**
* **18 matched**
* **2 mismatches**
* **90% match rate**

One property was recorded as **Occupied** without an active tenancy, while another was recorded as **Void** despite having an active tenancy.

### Pivot Table Summary

I used a Pivot Table to summarise reconciliation results by borough.

![02\_Occupancy\_Reconciliation\_By\_Borough](https://github.com/user-attachments/assets/65f6318f-259c-4f22-8ab6-ae8f0a31edf2)

*Two mismatches were identified in Ealing and Hounslow.*

---

## Tools Used

* Microsoft Excel
* XLOOKUP
* IF
* COUNTIF
* Conditional Formatting
* Pivot Tables
* Excel Tables

---

## Outcome

The review showed why record-level cross-checking is important. Overall totals can appear correct even when individual property records do not match.

[Download the Excel file](https://github.com/user-attachments/files/31519782/Project4_Part1_Occupancy_Reconciliation.xlsx)

## Next Part

**Part 2: Rent & Arrears Performance**





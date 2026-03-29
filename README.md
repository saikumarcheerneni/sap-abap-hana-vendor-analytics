# SAP ABAP on HANA — Vendor Performance Analytics

A full-stack SAP ABAP on HANA project built on a real S/4HANA system.

## System
- ABAP Release: 754
- Database: SAP HANA 2.00.052  
- System: S/4HANA on-premise

## Objects Built
| Object | Type | Description |
|---|---|---|
| ZCL_VENDOR_KPI_AMDP | ABAP Class | AMDP — SQLScript KPI calculation on HANA |
| ZI_VENDOR_PERFORMANCE | CDS View | Interface view — joins LFA1, EKKO, EKPO |
| ZC_VENDOR_PERFORMANCE | CDS View | Consumption view — Fiori UI annotations |
| ZSD_VENDOR_PERF | Service Definition | OData service definition |
| ZSB_VENDOR_PERF | Service Binding | OData V2 published endpoint |

## Architecture
```
DB Tables (LFA1, EKKO, EKPO, EKET)
        ↓
ZI_VENDOR_PERFORMANCE — Interface CDS View
        ↓
ZC_VENDOR_PERFORMANCE — Consumption CDS View
        ↓
ZSD_VENDOR_PERF — Service Definition
        ↓
ZSB_VENDOR_PERF — OData Service Binding
        ↓
SAP Fiori Launchpad
```

## Tech Stack
ABAP 754 · SAP HANA 2.0 · CDS Views · AMDP · OData · SAP Fiori

## Screenshots
![ADT Package](screenshots/01_adt_package.png)
![OData Metadata](screenshots/02_odata_metadata.png)
![Fiori Launchpad](screenshots/03_fiori_launchpad.png)

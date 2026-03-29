# Service Binding — ZSB_VENDOR_PERF

## Details
- Binding Type: OData V2 - UI
- Service Definition: ZSD_VENDOR_PERF
- Status: Published
- Service URL: /sap/opu/odata/sap/ZSB_VENDOR_PERF
- Entity Set: VendorPerformance

## OData Endpoint
VendorPerformance entity exposes:
- Vendor (key)
- VendorName
- Country
- AccountGroup
```

Save as `src\ZSB_VENDOR_PERF.md`

---

So your final `src` folder should have **5 files:**
```
src\
  ZCL_VENDOR_KPI_AMDP.abap
  ZI_VENDOR_PERFORMANCE.cds
  ZC_VENDOR_PERFORMANCE.cds
  ZSD_VENDOR_PERF.srvd
  ZSB_VENDOR_PERF.md
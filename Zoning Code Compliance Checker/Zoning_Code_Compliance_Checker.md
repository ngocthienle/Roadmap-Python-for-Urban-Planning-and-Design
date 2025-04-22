# 🏛️ Zoning Code Compliance Checker

A reproducible workflow for checking parcel‑level compliance with zoning regulations (FAR, BCR, setbacks, height limits) using modern Python libraries.

---

## 📘 I. Full Research Plan

### 1. Research Objectives
- **Evaluate** parcels for compliance with zoning regulations using open spatial data.  
- **Develop** reproducible, rule‑based models for detecting violations.  
- **Provide** actionable insight to planners for rezoning, policy intervention, or permitting.  

### 2. Data Requirements

| Dataset            | Description                                          | Format               |
| ------------------ | ---------------------------------------------------- | -------------------- |
| **Parcels**        | Lot boundaries with attributes (land area, use code) | Shapefile / GeoJSON  |
| **Buildings**      | Building footprints with height or number of floors  | GeoJSON / GeoPackage |
| **Zoning Map**     | Spatial zoning district codes                        | GeoJSON              |
| **Zoning Rules**   | Regulations per zone (e.g., FAR, setback, height)    | JSON or CSV          |

### 3. Metrics for Compliance

| Metric                | Description                              |
| --------------------- | ---------------------------------------- |
| **FAR**               | Building floor area ÷ parcel area        |
| **BCR**               | Building footprint area ÷ parcel area    |
| **Setback Compliance**| Distance from building to parcel boundary|
| **Height Limit**      | Actual vs. allowed building height       |
| **Lot Coverage**      | % of lot covered by structure            |

---

## 🛠️ II. Code Workflow

```mermaid
graph LR
  A[Input: Parcel, Building, Zoning layers] --> B[Preprocess & Join Spatial Layers]
  B --> C[Parse Zoning Code Rules (JSON)]
  C --> D[Apply Rule‑Based Compliance Checks]
  D --> E[Generate Violation Flags and Metrics]
  E --> F[Output: Interactive Map + Tables]
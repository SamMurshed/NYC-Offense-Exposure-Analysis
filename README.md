# NYC Offense Exposure Analysis Dashboard

An interactive data visualization dashboard that examines spatial variation in offense exposure across New York City boroughs. Built for health tech executives and applied researchers to inform location-aware risk modeling and resource allocation strategies.

## Project Overview

This dashboard analyzes a cleaned subset of NYPD complaint data (94 records) to reveal how offense exposure intensity varies geographically across NYC's five boroughs. The analysis focuses on spatial patterns rather than temporal trends or crime rates, providing exploratory insights for health tech applications.

**Key Finding:** Manhattan experiences 3.5x more offense incidents than Staten Island, despite similar offense type distributions across all boroughs—highlighting that exposure intensity, not offense composition, drives spatial variation.

## Demo
Deployment Link to See It Live: https://claude.ai/public/artifacts/e84b23ac-5de9-4521-9000-5374fa85b17f 

### Dashboard Walkthrough
![DBZGIF](https://github.com/user-attachments/assets/42796530-3581-4245-80a2-7377383b9e48)


## Features

### Six Interactive Sections
1. **Executive Summary** - High-level insights and health tech relevance
2. **Dataset Overview** - KPIs, borough distribution, and data constraints
3. **Borough Frequency Analysis** - Comparative offense counts with interpretations
4. **Composition Analysis** - Heatmap showing offense types across boroughs
5. **Statistical Context** - Chi-square test results with appropriate use guidance
6. **Strategic Implications** - Three-stage roadmap from exploration to deployment

### Design Principles
- **Insight-first**: Emphasizes "what this means" over "what this shows"
- **Executive-friendly**: Minimal jargon, clear visual hierarchy
- **Analytical credibility**: Transparent about limitations and appropriate use cases
- **Interactive exploration**: Tab-based navigation for depth without overwhelm

## Tech Stack

- **Frontend Framework:** React
- **Data Visualization:** Recharts (bar charts, pie charts, heatmaps)
- **Styling:** Tailwind CSS
- **Icons:** Lucide React
- **Statistical Analysis:** Chi-square test for spatial independence

## Dataset

- **Source:** Cleaned subset of NYPD complaint data
- **Records:** 94 offense incidents
- **Coverage:** All 5 NYC boroughs
- **Categories:** Homicide-Negligent (Unclassified & Vehicle-Related), Dangerous Drugs
- **Constraints:** 
  - No temporal dimension
  - No population denominators for rate calculation
  - No geographic coordinates for precise mapping
  - Exploratory/directional findings only

## Getting Started

### Prerequisites
```bash
node >= 14.0.0
npm >= 6.0.0
```

### Installation
```bash
# Clone the repository
git clone https://github.com/yourusername/nyc-offense-dashboard.git

# Navigate to project directory
cd nyc-offense-dashboard

# Install dependencies
npm install

# Start development server
npm start
```

The dashboard will open at `http://localhost:3000`

### Build for Production
```bash
npm run build
```

## Key Insights

### Spatial Variation
- **Manhattan:** 28 records (29.8% of total)
- **Brooklyn:** 24 records (25.5%)
- **Queens:** 18 records (19.1%)
- **Bronx:** 16 records (17.0%)
- **Staten Island:** 8 records (8.5%)

### Statistical Analysis
- **Chi-square test:** χ² = 5.844, df = 8, p = 0.665
- **Interpretation:** No significant association detected, likely due to small sample size rather than true absence of patterns

### Composition Findings
All three offense categories appear in every borough with similar proportional distributions, but Manhattan and Brooklyn consistently show higher absolute counts—suggesting volume-based rather than type-based variation.

## Use Cases for Health Tech

1. **Location-Aware Risk Modeling:** Integrate offense exposure as environmental stress proxy in mental health prediction models
2. **Targeted Resource Allocation:** Deploy crisis intervention and trauma-informed care to high-exposure areas
3. **Population Health Strategy:** Scale universal interventions by local exposure intensity rather than creating borough-specific programs

## Data Enrichment Roadmap

### Current State
- Directional spatial signal from subset data
- Limited to exploratory insights

### Next Steps
- Add temporal dimension for trend analysis
- Include population denominators for per-capita rates
- Expand offense category coverage

### Future Vision
- Link to health outcomes (ER visits, mental health utilization)
- Build predictive risk models
- Enable operational deployment for resource optimization


## 🙏 Acknowledgments

- NYPD for publicly available complaint data
- Health tech stakeholders who informed the dashboard design requirements
- Recharts library for flexible visualization components

---

**Note:** This analysis is exploratory in nature. Findings should be validated with larger datasets and appropriate population adjustments before informing policy or operational decisions.

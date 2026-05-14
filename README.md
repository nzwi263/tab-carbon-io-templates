# tab-carbon-io-templates

Templates for generating SaaS benchmarking reports using Carbon.io ECharts visualizations.

## Overview

This repository contains JSON templates for rendering ECharts-based charts that benchmark company metrics against peer groups. Each template defines company metadata, report details, user metrics, and chart configurations.

## Template Structure

Templates are organized under `templates/` with the following sections:

### Company Metadata
- `stage` - Company funding stage (e.g., Seed, Series A)
- `industry_sector` - Industry classification
- `country` - Operating country
- `currency` - Reporting currency

### Report Details
- `data_range_months` - Historical data window
- `reporting_year` - Year of reported data
- `no_peers_compared` - Number of peer companies in benchmark

### User Metrics
Key performance indicators including:
- Revenue growth rate
- Gross margin
- Runway
- Burn multiple
- Revenue per employee
- CAC payback

### Charts

Each metric includes an ECharts configuration with:
- **Box plots** showing distribution (Min, Q1, Median, Q3, Max)
- **Scatter plots** marking the company's position
- **Distribution curves** visualizing peer spread

Chart types:
- `revenue_growth_vs_mrr` - Scatter chart comparing MRR vs revenue growth
- `revenue_growth_rate`, `gross_margin`, `burn_multiple`, `revenue_per_employee`
- `valuation`, `mrr`, `capital_efficiency`, `runway_months`, `revenue_multiple`

## Usage

Templates are consumed by the TAB platform to generate benchmarking reports. Each template version is prefixed with a version tag (e.g., `v00-02`).

## Version

Current template version: `v00-02`
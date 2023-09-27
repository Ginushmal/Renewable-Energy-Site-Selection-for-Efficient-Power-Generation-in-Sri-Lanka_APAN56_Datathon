# Renewable Energy Site Selection for Efficient Power Generation in Sri Lanka - APAN56_Datathon

## Table of Contents
- [Introduction](#introduction)
- [Dataset Description](#dataset-description)
- [Contributors](#contributors)
- [Approach](#approach)
  - [Feature Engineering](#feature-engineering)
  - [Results](#results)
- [Conclusion](#conclusion)
- [Citations](#citations)

## Introduction

Welcome to the Renewable Energy Site Selection project, a solution developed for the APAN56 competition. This project addresses the challenge of identifying optimal locations for wind and solar energy projects in Sri Lanka. Leveraging a diverse dataset encompassing weather and geographical information, we aim to assist potential investors in the renewable energy sector. Our goal is to provide strategic recommendations for cities suitable for efficient power generation and attractive return on investment (ROI).

## Dataset Description

We utilized a comprehensive dataset that spans over 13 years, offering extensive weather-related data, solar data, wind data, and geographical attributes across multiple locations in Sri Lanka. This dataset enables us to explore long-term trends and seasonal variations, essential for informed decision-making.

## Contributors

We would like to acknowledge the valuable contributions of the following team members to this project:

- [Contributor 1](https://github.com/contributor1) (Role)
- [Contributor 2](https://github.com/contributor2) (Role)
- [Contributor 3](https://github.com/contributor3) (Role)
- [Contributor 4](https://github.com/contributor4) (Role)

## Approach

### Feature Engineering

Our project's success relied on thoughtful feature engineering, driven by both why and how we calculate each feature:

1. **Terrain Analysis**: We created this feature because locations with higher elevation variance require greater construction effort, thus incurring higher costs. To calculate it, we assessed the terrain by measuring elevation variances using OpenStreetMap data. Higher variance values indicate uneven terrains, which are less conducive to energy projects.

2. **Population Density**: By obtaining population density data, we evaluated potential user bases and the potential impact on the local community.

3. **Closest Highway Distance**: Using OpenStreetMap, we computed the distance to the nearest highways. Proximity to highways is crucial for transportation and can reduce construction costs.

4. **Nearby House Count**: To assess the impact on project construction, we counted buildings within a specified radius from each location.

5. **Daylight Duration**: Calculating daylight duration, while considering cloud cover, helped us estimate solar power generation potential.

6. **Annual Usable Wind Days Percentage**: We determined the percentage of days with wind speeds within the optimal range for wind energy generation.

7. **Wind Direction Variation**: Assessing wind direction stability aided in identifying locations with consistent wind patterns.

8. **High Radiation Days Percentage**: We evaluated the percentage of days with high solar radiation, crucial for solar energy generation.

9. **Solar Energy Loss Mean**: Calculations considered solar energy loss due to temperature coefficients.

10. **Distance to Substation**: Computed distance to the nearest substation to understand infrastructure costs.

11. **Irradiation**: We obtained irradiation data from an external source, a critical factor for solar power generation.

12. **Distance from Houses**: Determined the distance from populated areas to minimize potential disruptions.

13. **Distance from Roads**: We assessed the proximity to roads, impacting accessibility and construction logistics.

14. **Land Use Patterns**: Incorporating land use patterns based on a research study helped us understand land availability.

### Results

The AHP model provided values for each feature, which we used to calculate weighted sums of the rating values for each location. Locations with higher weighted sum values are considered more suitable for building renewable power plants.

## Conclusion

Our solution leverages data-driven insights to guide renewable energy site selection in Sri Lanka, facilitating efficient power generation and attractive ROI. We believe our strategic recommendations will benefit investors and contribute to sustainable energy development in the region.

## Citations

1. [Solar PV Power Plant Site Selection using a GIS-AHP based approach with application in Saudi Arabia](https://doi.org/10.1016/j.apenergy.2017.10.024)
2. [Solar Panel Efficiency](https://blog.ecoflow.com/za/solar-panel-efficiency/)
3. [Measuring the Temperature Coefficients of a PV Module](https://sinovoltaics.com/solar-basics/measuring-the-temperature-coefficients-of-a-pv-module/)
4. [Multi-criteria Decision Analysis for Wind Power Plant Location Selection](https://doi.org/10.1007/s10668-021-01438-5)
5. [Renewable Energy Resources and Technologies Applicable to Sri Lanka](#)
6. [AHP Calculation Methods](https://www.spicelogic.com/docs/ahpsoftware/intro/ahp-calculation-methods-396)
7. [Sri Lanka Wind Farm Analysis and Site Selection Assistance](#)

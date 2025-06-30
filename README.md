# Flu Risk Forecasting
*This project was completed as part of the [CareerFoundry Data Analytics Programme](https://careerfoundry.com/en/courses/become-a-data-analyst/).*

## Overview
A medical staffing agency that supplies temporary personnel to clinics and hospitals across the United States is preparing for the upcoming 2018/19 influenza season. The project analyses historical influenza and population data to identify high-risk population groups through correlation analysis between age and mortality, examine seasonal patterns to determine the start and end of flu season, and develop a state-level risk profile to forecast when, where, and how many staff would likely be required.
<br><br>

## Tools
- **Excel** - Data Preparation | Analysis
- **Tableau** - Forecasting | Visualisation | Storytelling
<br><br>

## Process
- **Data Preparation** - Data Exploration | Description | Profiling | Cleaning | Transformation & Integration
- **Analysis** - Descriptive Statistics | Statistical Analysis | Hypothesis Testing | Trend Analysis | Forecasting
- **Communication** - Visualisation | Storytelling
<br><br>

## Data
This analysis uses publicly available data sourced from the Centers for Disease Control and Prevention (CDC) and the US Census Bureau, covering the period from 2009 to 2017. The data was provided by CareerFoundry as part of their Data Analytics programme.

- [**Influenza-related deaths**](https://coach-courses-us.s3.amazonaws.com/public/courses/da_program/CDC_Influenza_Deaths_edited.xlsx) - Number of deaths by location, time, and age.
- [**Population**](https://coach-courses-us.s3.amazonaws.com/public/courses/data-immersion/A1-A2_Influenza_Project/Census_Population_transformed_202101.csv) - Number of people by location, time, age, and gender.
<br><br>

## Deliverables
- [**Interactive Tableau Storyboard**](https://public.tableau.com/views/MedicalStaffingPlan_17430147849920/Story1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)
<br><br>

## Key Insights
### 1. Vulnerable Populations
Adults aged 65 and older account for the vast majority of influenza-related deaths and display the greatest variation in mortality.

<table>
<tr>
<td align="center" valign="top" width="50%">
    <img src="visualisations/pie_deaths_age.png" ><br>
    <em>Adults aged 65 and older account for more than 60% of all influenza-related deaths — a trend that reinforces CDC classifications of this group as high risk.</em>
</td>
<td align="center" valign="top" width="50%">
    <img src="visualisations/scatter_correlation.png" ><br>
    <em>There is a strong positive correlation between population size and influenza-related deaths among older adults, particularly those aged 65+. This relationship weakens in younger groups, where mortality is lower and data suppression increases uncertainty.</em>
</td>
</tr>
</table>
<br>

### 2. Seasonality
Although the annual severity of influenza varied considerably, peak mortality consistently occurred in January, with Southern states often reporting the highest totals.

<table>
<tr>
<td align="center" valign="top" width="50%">
    <img src="visualisations/line_region_yearly.png" ><br>
    <em>Influenza deaths rise in November, peak sharply in January, and decline through April. The South consistently reports the highest mortality, while other regions follow near-identical trends.</em>
</td>
<td align="center" valign="top" width="50%">
    <img src="visualisations/bar_deaths_year.png" ><br>
    <em>The average annual death count across the period is 73,158 but varies significantly year to year with notable surges in 2014 and 2015.</em>
</td>
</tr>
</table>
<br>

### 3. Risk Classification & Forecasting
Allocating risk based on the size of each state’s elderly population revealed greater seasonal variability in deaths among high-risk states, reinforcing the case for prioritised resource allocation.

<table>
<tr>
<td align="center" valign="top" width="50%">
    <img src="visualisations/map_vulnerable.png" ><br>
    <em>Geospatial view confirms that high-risk populations are not confined to the South — with large vulnerable populations in California, the Northeast, and parts of the Midwest.</em>
</td>
<td align="center" valign="top" width="50%">
  <img src="visualisations/bar_risk_population.png" ><br>
  <em>Population size of age group 65+ across U.S. states categorised by risk profile — high-risk states have exponentially larger elderly populations.</em>
</td>
</tr>
<tr>
<td align="center" valign="top" width="50%">
    <img src="visualisations/line_risk_yearly.png" ><br>
    <em>Plotting seasonal mortality trends using the state-level risk profile revealed that high-risk states experienced the most pronounced surges, while low-risk states exhibited more moderate fluctuations — confirming the need for more resources during peak season. </em>
    </td>
<td align="center" valign="top" width="50%">
    <img src="visualisations/line_risk_forecast.png" ><br>
    <em>The forecast shows sharp seasonal peaks in high-risk states, reinforcing expectations of a heavier burden in these areas. In contrast, low-risk states display minimal fluctuation, suggesting a lower anticipated need for supplementary staffing.</em>
</td>
</tr>
</table>
<br>

## Takeaways
### Successes
The project delivered actionable insights into the geographic distribution of vulnerable populations and seasonal timing, enabling the development of a risk profile to guide strategic staffing decisions.

### Challenges
The available data lacked sufficient detail to account for all known risk factors in the analysis. In particular, the suppression of records for children under 5 limited risk assessment for this group, highlighting how data privacy laws can constrain public health analysis when key demographics are excluded.

### Way Forward
Moving forward, it is essential to recognise how privacy constraints may limit access to critical data. When such limitations arise, efforts should focus on identifying alternative sources and adopting alternative methodologies to address gaps. Maintaining adaptability in analytical approaches will help ensure that insights remain robust and ethically sound, even when datasets are incomplete.

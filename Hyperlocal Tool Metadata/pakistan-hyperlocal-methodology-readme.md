# Pakistan Community Vulnerability Score (Methodology)

## Overview
Average community vulnerability score on a scale of 3 to 15, where higher values represent higher levels of vulnerability, based on communities’ 1) exposure risk, 2) comorbidities risk, and 3) other vulnerabilities.

## Components Included

### 1. Exposure

Exposure components include equally weighted indicators of: 

| # | **Variable**      | **Variable Description**  | **Source** |
| ------------- |-------------| -----| -----|
| 1 | <code>Community density</code>      | Community density at the 1 km squared level| Demographic and Health Survey (DHS), 2018 |
| 2 | <code> Healthcare workforce size</code>      |  Percentage of adults aged 15 to 49 employed in health care or essential services| Demographic and Health Survey (DHS), 2018 |
| 3 | <code> Number of household members per sleeping room</code>      |  Average number of household members per sleeping room| Demographic and Health Survey (DHS), 2018 |
| 4 | <code> Percentage of intergenerational households</code>      |  Percentage of households that are intergenerational, defined as having a a youth under the age of 18 and an elder aged 60 or older | Demographic and Health Survey (DHS), 2018 |
| 5 | <code> Provincial cumulative COVID-19 cases </code>      |   Rate of accumulated COVID-19 cases to population at the province level | Government of Pakistan COVID-19 dashboard |
| 6 | <code> Social Mixing </code>      |   Change in visits retail and recreation locations, public transport sites, and workplaces at the province level | Google mobility data |
| 7 | <code> Refugee Population </code>      |   Number of registered refugees at camps and urban locations. | UNHCR |




### 2. Comorbidities

The comorbidities component includes equally weighted indicators of:
| # |**Variable**      | **Variable Description**  | **Source** |
| ------------- |-------------| -----| -----|
| 1 | <code> Elderly population aged 60+</code>      | Elderly population aged 60 and older | Demographic and Health Survey (DHS), 2018 |
| 2 | <code> Female adult obesity burden</code>      |  Rate of female adult (15-49) obesity | Demographic and Health Survey (DHS), 2018 |

### 3. Vulnerabilities

The vulnerabilities component is based on equally weighted indicators for:

| # |**Variable**      | **Variable Description**  | **Source** |
| ------------- |-------------| -----| -----|
| 1 | <code> Information access</code>      | Two indicators are equally weighted within the information access sub-component: 1) percentage of households with no cell phones in the household, and 2) percentage of households with no radio, internet, or television and no adults aged 15 to 49 who regularly consume traditional media (newspaper, radio, television). Regular consumption is defined as reading, listening, or watching the media at least once a week.  | Demographic and Health Survey (DHS), 2018 |
| 2 | <code> Vaccination likeliness </code>      |  Three indicators are equally weighted within the vaccination likeliness sub-component: 1) percentage of population in the bottom quintile of the DHS wealth index; 2) percentage of women who have given birth who have not received any tetanus vaccinations; and 3) percentage of female household members who have not been to a health facility or been visited by a field worker in the last year.  | Demographic and Health Survey (DHS), 2018 |
| 3 | <code> Prevention </code>      |    Two indicators are equally weighted within the prevention sub-component: 1) percentage of individuals with no soap available for handwashing inside the household, and 2) percentage of individuals with no water available for handwashing inside the household. | Demographic and Health Survey (DHS), 2018 |


### 4. Calculation
Indicators within components and sub-components are combined with z-scores at the 1 km squared grid level. The total of all z-scores is then classified into a component and sub-component score ranging from 1 to 5 by quintile. Sub-components are added together and classified into a component score ranging from 1 to 5 by quintile. All three components are then added together.


### 5. Output Source:
Source: [Fraym](https://fraym.io/)
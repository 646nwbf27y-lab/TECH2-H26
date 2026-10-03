# Norwegian municipalities

| Column | Description and unit |
| --- | --- |
| `muni_id` | Official four-character municipality code; a string with leading zeros preserved. |
| `municipality` | Full official municipality name. |
| `population` | Number of residents on January 1 of `pop_year`. |
| `land_area` | Land area in km², excluding freshwater, in `pop_year`. |
| `mean_age` | Mean age of residents, in years, on January 1 of `age_year`. |
| `median_age` | Median age of residents, in years, on January 1 of `age_year`. |
| `college_share` | Percentage of residents aged 16+ with short or long higher education on October 1 of `edu_year`. The denominator excludes residents with unknown or no completed education; this is the sum of the two published percentages, on a 0–100 scale. |
| `median_income` | Median annual household income after tax, in NOK, for `income_year`. Excludes student households and children under 18 living alone. This is household income, without adjustment for household size. |
| `cars` | Number of registered passenger cars on December 31 of `cars_year`, across all transport uses and fuels. |
| `electric_cars` | Number of those passenger cars powered by electricity, excluding hybrids. From 2025, vehicles with registered lessees are assigned to the lessee's municipality; earlier figures used the owner's municipality. This change applies to both vehicle counts. |
| `pop_year` | Actual reference year of population and land area; also determines which municipalities appear. |
| `age_year` | Actual reference year of mean and median age. |
| `edu_year` | Actual reference year of educational attainment. |
| `income_year` | Actual calendar year of household income. |
| `cars_year` | Actual reference year of both vehicle counts. |

Empty fields indicate missing or unavailable observations. Source years can differ.
Rows are ordered by population from largest to smallest, then municipality code.

Population density is not included. Calculate residents per km² of land as
`population / land_area` when needed. The land area figures are rounded to whole km².

Sources: Statistics Norway (SSB):

- [11342: Population and area](https://www.ssb.no/en/statbank/table/11342)
- [13536: Mean and median age](https://www.ssb.no/en/statbank/table/13536)
- [09429: Educational attainment](https://www.ssb.no/en/statbank/table/09429)
- [06944: Household income](https://www.ssb.no/en/statbank/table/06944)
- [07849: Registered vehicles by fuel](https://www.ssb.no/en/statbank/table/07849)

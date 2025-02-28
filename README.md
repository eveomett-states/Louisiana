# Louisiana Election Shapefile

This shapefile was processed by Professor Ellen Veomett and her student Arbie Hsu.

# **Sources**

The following obtained from [Redistricting Data Hub](https://redistrictingdatahub.org/) on June, 2024:

[Population data](https://redistrictingdatahub.org/dataset/louisiana-block-pl-94171-2020-by-table/): based on the decennial census at the Census Block level on 2020 Census Redistricting Data

[Congressional District data](https://redistrictingdatahub.org/dataset/2022-louisiana-congressional-districts-approved-plan/): 2022 Congressional Districts Approved Interim Plan

[State House District data](https://redistrictingdatahub.org/dataset/2022-louisiana-state-house-of-representatives-approved-plan/): 2022 State House Approved Interim Plan

[State Senate District data](https://redistrictingdatahub.org/dataset/2022-louisiana-state-senate-approved-plan/): 2022 State Senate Districts Interim Plan from

[2020 election data](https://redistrictingdatahub.org/dataset/vest-2020-louisiana-precinct-and-election-results/): VEST 2020 precinct and election results

[2019 election data](https://redistrictingdatahub.org/dataset/vest-2019-louisiana-precinct-boundaries-and-election-results-shapefile/): VEST 2019 precinct and election results

[2018 election data](https://redistrictingdatahub.org/dataset/vest-2016-georgia-precinct-and-election-results/): VEST 2018 precinct and election results

[2016 election data](https://redistrictingdatahub.org/dataset/vest-2016-louisiana-precinct-and-election-results/): VEST 2016 precinct and election results

# **Processing**

Demographic data were aggregated from the census block level and precincts were assigned to districts using [MGGG's proration software](https://github.com/mggg/maup). Election data were also prorated onto VTDs from the original precinct shapefile using the `maup` package.

# **Metadata**

Below is a brief description of each of the listed variables in the attribute table of the VTD shapefile:

- `STATEFP20`: State FIPS code of 2020
- `COUNTYFP20`: County FIPS code of 2020
- `VTDST20`: Voting tabulation district FIPS code of 2020
- `GEOID20`: VTD FIPS code of 2020
- `NAME20`: Voting tabulation district name of 2020
- `CD`: Congressional district ID in 2022 enacted congressional map
- `SEND`: State Senate district for 2022 State Senate Adopted Plan
- `HDIST`: State House district for 2022 State House of Representatives Districts Plan
- `TOTPOP`: Total population in 2020 Census
- `NH_WHITE`: White, non-hispanic, population in 2020 Census
- `NH_BLACK`: Black, non-hispanic, population in 2020 Census
- `NH_AMIN`: American Indian and Alaska Native, non-hispanic, population in 2020 Census
- `NH_ASIAN`: Asian, non-hispanic, population in 2020 Census
- `NH_NHPI`: Native Hawaiian and Pacific Islander, non-hispanic, population in 2020 Census
- `NH_OTHER`: Other race, non-hispanic, population in 2020 Census
- `NH_2MORE`: Two or more races, non-hispanic, population in 2020 Census
- `HISP`: Hispanic population in 2020 Census
- `H_WHITE`: White, hispanic, population in 2020 Census
- `H_BLACK`: Black, hispanic, population in 2020 Census
- `H_AMIN`: American Indian and Alaska Native, hispanic, population in 2020 Census
- `H_ASIAN`: Asian, hispanic, population in 2020 Census
- `H_NHPI`: Native Hawaiian and Pacific Islander, hispanic, population in 2020 Census
- `H_OTHER`: Other race, hispanic, population in 2020 Census
- `H_2MORE`: Two or more races, hispanic, population in 2020 Census
- `VAP`: Total voting age population in 2020 Census
- `HVAP`: Hispanic voting age population in 2020 Census
- `WVAP`: White, non-hispanic, voting age population in 2020 Census
- `BVAP`: Black, non-hispanic, voting age population in 2020 Census
- `AMINVAP`: American Indian and Alaska Native, non-hispanic, voting age population in 2020 Census
- `ASIANVAP`: Asian, non-hispanic, voting age population in 2020 Census
- `NHPIVAP`: Native Hawaiian and Pacific Islander, non-hispanic, voting age population in 2020 Census
- `OTHERVAP`: Other race, non-hispanic, voting age population in 2020 Census
- `2MOREVAP`: Two or more races, non-hispanic, voting age population in 2020 Census
- `AGR19D`:  Number of votes for 2019 Democratic Commissioner of Agriculture
- `AGR19R`:  Number of votes for 2019 Republican Commissioner of Agriculture
- `AGR19O`:  Number of votes for 2019 other party's Commissioner of Agriculture
- `ATG19D`: Number of votes for 2019 Democratic attorney general candidate
- `ATG19R`: Number of votes for 2019 Republican attorney general candidate
- `ATG19O`: Number of votes for 2019 other party's attorney general candidate
- `AUD19R`: Number of votes for 2019 Republican Auditor
- `AUD19O`: Number of votes for 2019 other party's Auditor
- `AUD19R`: Number of votes for 2019 Republican Auditor
- `GOV19D`: Number of votes for 2019 Democratic gubernatorial candidate
- `GOV19R`: Number of votes for 2019 Republican gubernatorial candidate
- `GOV19O`: Number of votes for 2019 other party's gubernatorial candidate
- `PRE16D`: Number of votes for 2016 Democratic President
- `PRE16O`: Number of votes for 2016 other party's President
- `PRE16R`: Number of votes for 2016 Republican President
- `PRE20D`: Number of votes for 2020 Democratic President
- `PRE20R`: Number of votes for 2020 Republican President
- `PRE20O`: Number of votes for 2020 other party's President
- `SOS19D`: Number of votes for 2019 Democratic Secretary of State
- `SOS19R`: Number of votes for 2019 Republican Secretary of State
- `TRE19D`: Number of votes for 2019 Democratic Treasurer
- `TRE19R`: Number of votes for 2019 other party's Treasurer
- `USS16D`: Number of votes for 2016 Democratic senate candidate
- `USS16R`: Number of votes for 2016 Republican senate candidate
- `USS20D`: Number of votes for 2020 Democratic senate candidate
- `USS20R`: Number of votes for 2020 Republican senate candidate
- `USS20O`: Number of votes for 2020 other party's senate candidate

# **Projection**

The shapefile uses a UTM NAD83 projection (EPSG: 4269).

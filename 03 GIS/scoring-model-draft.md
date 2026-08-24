# FireSafe Atlas Scoring Model — Draft (Neil Panchal)

**Status: draft, pending Emma's equity/bias review before any final maps are built.**

The FireSafe score is an educational planning-support index built from public data. It does not replace official fire warnings, evacuation orders, emergency management guidance, or local professional assessment. It shows patterns of risk and need for preparedness support, not a prediction of where a fire will happen.

Every layer uses a simple 1 to 3 scale so a non-technical reader can understand it:

- **1 = Lower relative concern**
- **2 = Moderate relative concern**
- **3 = Higher relative concern**

These scores are always relative to other areas within the Butte County study area, not an absolute national or global ranking.

## 1. Fire exposure

What it measures: how much recent and historical fire activity has touched this area.

- **1** — No or very limited recorded fire history nearby (CAL FIRE FRAP perimeters) and low NASA FIRMS hotspot density in the last 10 years.
- **2** — Some recorded fire history nearby, or moderate hotspot density, but not within a recent major fire perimeter.
- **3** — Within or adjacent to a mapped historical fire perimeter (such as the 2018 Camp Fire boundary) or has high recent hotspot density.

Source: CAL FIRE FRAP fire perimeters, NASA FIRMS active fire hotspots.

## 2. Environmental stress

What it measures: vegetation, fuel, and dry/hot conditions that can make fire behavior more severe.

- **1** — Land cover is mostly low-fuel (built-up, cropland, or sparse vegetation) with unremarkable NDVI and temperature/precipitation patterns.
- **2** — Mixed fuel types (some tree cover or shrubland) or moderately elevated heat/dryness signals.
- **3** — Dense tree cover or shrubland fuel type combined with NDVI or NASA POWER data showing drought or heat stress.

Source: ESA WorldCover land cover, MODIS NDVI, NASA POWER.

## 3. Population exposure

What it measures: how many people live in the area and their relative social vulnerability, using support-focused framing, not deficit framing.

- **1** — Lower population density and lower CDC/ATSDR SVI ranking relative to the rest of the study area.
- **2** — Moderate population density or moderate SVI ranking.
- **3** — Higher population density, higher SVI ranking, or both, indicating greater potential need for preparedness support.

Source: WorldPop gridded population, CDC/ATSDR Social Vulnerability Index, US Census ACS.

## 4. Road / evacuation access

What it measures: how well-connected an area is by road, as a proxy for how easily people could evacuate.

- **1** — Multiple through-roads or short distance to a state highway.
- **2** — One clear through-road, or moderate distance to a state highway.
- **3** — Limited road connectivity (dead-end or single-road access) or long distance to a state highway. This reflects Butte County's canyon and ridge terrain, which was a major factor in the Camp Fire evacuation.

Source: OpenStreetMap road network, US Census TIGER/Line for reference boundaries.

This layer is a general access indicator only. It must never be used to tell anyone which specific evacuation route is safe, per the project's Do/Don't rules.

## 5. Emergency-service access

What it measures: distance to the nearest documented hospital, clinic, or fire station.

- **1** — Short distance to a licensed healthcare facility and a known fire station or CAL FIRE unit.
- **2** — Moderate distance to the nearest documented facility.
- **3** — Long distance to the nearest documented facility, indicating a potential gap in emergency response time.

Source: California HCAI Licensed Healthcare Facility Listing, OpenStreetMap fire station tags (CAL FIRE unit locations to be added in Week 5 if a clean public source is found).

## 6. Community assets

What it measures: presence of schools and community gathering places nearby, which matter for both daily life and emergency sheltering potential.

- **1** — One or more schools or community facilities within a short distance.
- **2** — At least one facility within a moderate distance.
- **3** — No documented school or community facility within a reasonable distance.

Source: California Department of Education Public School Directory, California HCAI facility listing.

Note: a score of 3 here reflects a documented data gap in nearby services, not a judgment about the community itself.

## What's next

These six layers get combined into a single composite FireSafe score in Week 8, using the weights in `scoring-weights.csv`. Both this draft and the weights file go to Emma for equity/bias review before any layer is finalized into a map.

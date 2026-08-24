# Final Study Area Memo — Neil Panchal

**Status: Conditional Phase 1 pilot region.** This is a practical implementation decision based on currently available public data, approved by Rhea Ghosal for Week 4 technical work. It is not a final equity or community endorsement. It remains conditional pending Emma's ethics/equity review and Lauren's environmental context review, both still outstanding.

## Selected region

**Concow, Magalia, and Paradise, Butte County, California.** These are unincorporated, rural mountain communities in the Sierra Nevada foothills northeast of Chico.

## Population

Butte County has an estimated population of roughly 208,000 to 209,000 people countywide (2024-2025 Census/ACS estimates). The pilot focus communities are much smaller: Concow and Magalia are unincorporated mountain communities, and Paradise's population dropped sharply after 2018 and is still rebuilding. Exact tract-level population figures for the pilot area will come from WorldPop and Census ACS data pulled in Week 5.

## The wildfire problem

This area was the site of the 2018 Camp Fire, the deadliest and most destructive wildfire in California history: 85 deaths and more than 18,000 structures destroyed. The fire moved through Concow, Paradise, and Magalia and forced the evacuation of roughly 40,000 people. Butte County's terrain, steep canyons and ridgelines that divide the county into separated regions with limited through-roads, made evacuation and emergency response especially difficult, and that same terrain challenge persists today for any future fire.

## Rural and underserved relevance

Concow and Magalia are unincorporated communities with older housing stock and more limited access to services than nearby incorporated cities. This is a community that public data shows may need more preparedness support, not a community that caused its own risk. The CDC/ATSDR Social Vulnerability Index will be used in Week 5 to identify which specific census tracts in the study area show the greatest need for support across poverty, age, disability, vehicle access, and language-access indicators. Any description of this need in the dashboard or final report will use support-focused language (for example, "communities with greater need for preparedness support") rather than deficit-framed language, per the project's Do/Don't rules.

## Data limitations

Several limitations apply to this study area and should be stated plainly in the dashboard:

- **Fire history is well documented but not exhaustive.** CAL FIRE FRAP describes its own historical perimeter dataset as the most complete available but still incomplete; the absence of a mapped perimeter somewhere does not mean no fire occurred there.
- **Boundaries.** GADM was used only for early region screening in Week 3 and is not licensed for redistribution in a public dashboard. US Census TIGER/Line boundaries (public domain) will be used instead for anything the public actually sees.
- **Air quality monitoring is sparse.** Butte County has only 3 official CARB-operated monitoring stations plus supplemental PurpleAir sensors, so smoke/AQI readings may not reflect conditions in every specific community, especially remote areas like Concow.
- **Community assets data is a mix of sources.** Schools come from the CA Department of Education's official directory; hospitals and clinics come from the CA HCAI licensed facility listing. Both are more reliable than crowd-sourced tagging, but neither includes informal community gathering spaces or fully captures newer facilities built since the Camp Fire.
- **Butte County has already been extensively studied** by researchers, journalists, and government agencies following the Camp Fire. FireSafe Atlas should cite and build on that existing work rather than duplicating it, and should be clear that it is not the first or only source of information about this community's wildfire risk.
- **This region choice is conditional.** It reflects data availability and technical feasibility, not a completed ethics or environmental review. If Emma's or Lauren's review raises a serious concern, the pilot may need to shift to the backup region (Mescalero Apache Reservation / Ruidoso, New Mexico) identified in `pilot-region-recommendation.md`.

## What happens next

Once this memo and the scoring framework (`scoring-model-draft.md`, `scoring-weights.csv`) are drafted, both go to Emma for equity/bias review before any final maps are built, per the Week 4 task list.

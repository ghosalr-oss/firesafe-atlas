# Pilot Region Recommendation — Neil Panchal

**Status: conditional pending ethics and environmental review.** Rhea Ghosal has approved Butte County as the conditional Phase 1 pilot region so Week 4 technical work (study area memo, scoring model, scoring weights) can proceed. This is a practical implementation decision based on data availability and feasibility, not a final equity or community endorsement. It has not yet incorporated Emma's equity notes or Lauren's environmental context notes, since neither exists in the repo yet as of this writing. Mapping of the backup region (Mescalero Apache Reservation / Ruidoso) should not begin without a separate ethics, data-governance, and community-context review.

## The three candidates

1. **Concow / Magalia / Paradise area, Butte County, California** — site of the 2018 Camp Fire, the deadliest wildfire in California history. Rural, lower-income mountain communities.
2. **Mescalero Apache Reservation / Ruidoso area, Lincoln and Otero Counties, New Mexico** — site of the 2024 South Fork and Salt Fires, which started on tribal trust land and forced roughly 5,000 evacuations.
3. **Mati and nearby rural wildland-urban interface villages, Attica, Greece** — site of the 2018 Mati wildfire, one of the deadliest wildfires in modern European history, with a large elderly population and informally developed roads.

Full comparison is in `pilot-region-data-availability-matrix.csv`.

## Preliminary primary recommendation: Butte County, California

Butte County has the strongest, most complete data across every category in the matrix: fire history, population, roads, boundaries, community assets, environmental data, and air quality all have solid public sources with no major gaps. That means the team can move quickly from data to map to dashboard without getting stuck on missing or hard-to-access data during the pilot phase. It's also a real, well-documented case of a rural, lower-income community facing catastrophic wildfire risk, so it's genuinely impactful, not just convenient.

The tradeoff: Butte County and the Camp Fire have already been studied extensively by researchers, journalists, and government agencies. FireSafe Atlas would be adding to a crowded body of work rather than filling a clear gap.

## Preliminary backup recommendation: Mescalero Apache Reservation / Ruidoso, New Mexico

This region is a stronger test of the project's actual mission, since tribal land is exactly the kind of underserved, under-mapped community FireSafe Atlas is meant to help. It has real, recent wildfire relevance from the 2024 South Fork and Salt Fires. But the data gaps are real too: OpenStreetMap and standard boundary sources noticeably under-represent tribal land, so building this pilot would take more upfront work to source tribal-specific boundary and roads data before any scoring could begin.

## Why Attica, Greece was not selected as primary or backup

It's a compelling case for testing global replication, but it requires substituting two entire data categories (social vulnerability index and air quality) with non-US sources that haven't been vetted yet. That's a bigger research lift than the team can absorb during the pilot phase. It may be worth revisiting for the replication guide later in the project, once the core scoring model is proven on a US region.

## Before this is finalized

Read and incorporate:
- Emma's equity notes on which candidate region is most ethically appropriate to publicly map (especially relevant for the tribal land case, given data sovereignty concerns).
- Lauren's environmental and community relevance notes on ecosystem type, wildfire seasonality, and whether local schools/community centers are relevant to the smoke-day guide.

If either flags a serious concern with Butte County as primary, the Mescalero/Ruidoso region is the next-most-feasible option, with the understanding that Week 2's source tracker will need tribal-specific boundary and roads sources added before scoring can start.

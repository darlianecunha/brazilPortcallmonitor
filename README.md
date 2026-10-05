# Brazil Port Call Monitor

**How long cargo ships wait and stay at Brazilian ports, and how large they are: annual medians for 103 port installations, built from 215,212 ANTAQ cargo calls (2019-2025) linked to vessel deadweight**

[![Live site](https://img.shields.io/badge/Live-brazil--portcallmonitor.vercel.app-2ea44f)](https://brazil-portcallmonitor.vercel.app)
[![Part of Brazil Port Data](https://img.shields.io/badge/Part%20of-brazilportdata.com-0b2239)](https://www.brazilportdata.com)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

## What this is

Port performance in Brazil is usually reported as tonnes moved. This monitor looks at the ships instead: how many cargo calls each installation receives, how long vessels wait at anchorage before berthing, how long they stay at berth and how large they are. Call records from ANTAQ are linked to each vessel's deadweight through its IMO number.

| Indicator, Brazil | 2019 | 2025 |
|---|---|---|
| Cargo calls | 29.5 thousand | 32.1 thousand (+9%) |
| Median waiting time before berthing | 9.7 h | **17 h** |
| Median time at berth | 34 h | 36 h |
| Median vessel size | 52 kt DWT | 58 kt DWT |
| Cargo handled | | 1,316 Mt (+26%) |

The headline finding: calls grew by 9%, but the median wait before berthing almost doubled. Dry bulk carries most of the delay (median 49 h of waiting in 2025), against 26 h for liquid bulk, 7.6 h for general cargo and 5.2 h for containers.

## What the page shows

| Section | Content |
|---|---|
| **Headline figures** | Calls, median waiting time, median time at berth, median vessel size and cargo, 2025 against 2019 |
| **Trends by segment** | Calls per year and median waiting time for dry bulk, liquid bulk, container and general cargo |
| **Port profiles** | For any of the 103 installations: calls per year, cargo mix, median waiting time (T1) and time at berth (TA) over 2019-2025 |
| **Port ranking** | Installations ranked by calls, waiting time, time at berth or vessel size; click a bar to open the profile |

## Method notes

- **Scope:** 215,212 cargo-handling calls in deep-sea and cabotage navigation with departure between 2019 and 2025, at 141 installations. Profiles and rankings cover the 103 installations with 100 or more calls.
- **Source:** ANTAQ *Estatístico Aquaviário* (open data). Vessel deadweight linked by IMO number from public ship registers. Figures are aggregated by Brazil Port Data.
- **Waiting time (T1)** follows ANTAQ's definition: arrival at the anchorage area to berthing, including transit through the access channel. **Time at berth (TA)** runs from berthing to unberthing. Records above 720 h are excluded from the time medians.
- **Segment** is the cargo nature with the largest weight in each call; container calls are separated from general cargo.
- **Disclosure control:** annual values based on fewer than 10 calls are not shown.
- **Scope difference:** cargo here covers deep-sea and cabotage calls only, so it is lower than the all-navigation total in the [Brazil Ports & Terminals Explorer](https://github.com/darlianecunha/brazilport20) (1,403 Mt in 2025).
- **Coming next:** at-berth CO₂ by installation, from a method currently under peer review.

## Repository map

| Path | Content |
|---|---|
| `index.html` | The whole application: page, aggregated annual medians and charts in one file |

Only aggregated annual figures are published. Call-level records are not included in this repository.

## How to cite

> Cunha, D. R. (2026). *Brazil Port Call Monitor*. Brazil Port Data. https://brazil-portcallmonitor.vercel.app

## Detailed analyses

Berth- and terminal-level waiting and berth times by segment and season, fleet profiles, at-berth CO₂ inventories with shore-power potential and benchmarking against Brazilian and European peer ports are available on request: darliane@brazilportdata.com

## Related projects

- [brazilportdata](https://github.com/darlianecunha/brazilportdata): the hub site for all Brazil Port Data panels
- [brazilport20](https://github.com/darlianecunha/brazilport20): cargo by installation, 2021-2025
- [antaq-port-statistics](https://github.com/darlianecunha/antaq-port-statistics): open dataset of annual ANTAQ statistics, including mean port times
- [maritimeco2](https://github.com/darlianecunha/maritimeco2): at-berth CO₂ estimation (IMO Fourth GHG Study method)

## Author and licence

**Darliane Ribeiro Cunha, PhD**. [ribeirocunha.com](https://ribeirocunha.com) · [ORCID 0000-0003-2548-1237](https://orcid.org/0000-0003-2548-1237)

Page and analysis: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Data: ANTAQ open data and public ship registers.

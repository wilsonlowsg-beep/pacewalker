# Pacewalker

Safer walking routes to school in Singapore.

Enter a home postal code, pick a school, polytechnic or ITE college within 10 km, and Pacewalker compares the fastest walking route with the safest one. Every road crossing is scored by the size of the road and whether it has traffic lights, a marked crossing or nothing at all. Overhead bridges and underpasses count as protected crossings. The app also shows School Zones, Silver Zones and how much of each walk is under a covered linkway.

Inspired by Safewalkr, built by three Thomas Jefferson High School students for Fairfax County, Virginia.

## How the safety score works

- Road crossings are weighted by road size (estate road → arterial road) and protection (traffic lights, marked crossing, none).
- Crossings inside a School Zone or Silver Zone carry 25% less risk because of lower speed limits and traffic calming.
- Walking along a carriageway, through car parks, and past side-road junctions adds smaller penalties.
- Score = 100 × e^(−risk/30).

Always walk a new route with your child before relying on it.

## Data sources

- Walking routes: [Valhalla](https://valhalla1.openstreetmap.de) (FOSSGIS), on OpenStreetMap data
- Crossing details: OpenStreetMap via the Overpass API, © OpenStreetMap contributors (ODbL)
- Base map and address search: [OneMap](https://www.onemap.gov.sg), Singapore Land Authority
- School list: Ministry of Education, via [data.gov.sg](https://data.gov.sg)
- School Zones, Silver Zones, covered linkways, overhead bridges/underpasses and road crossings: [LTA DataMall](https://datamall.lta.gov.sg) static datasets (Apr 2025 / Sep 2026)

Contains information from datasets accessed via data.gov.sg and LTA DataMall, made available under the terms of the Singapore Open Data Licence version 1.0.

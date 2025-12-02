# Capital Slice: Briefing on Key Business Elements

## Business Overview

You and your partners operate **Capitol Slice**, a premium pizza-by-the-slice operation in Washington DC. Your fleet consists of two mobile food trucks serving high-quality, fresh-baked pizza with fresh ingredients. The operation initially is focused on Saturdays—a strategic focus on peak weekend activity.

Every Thursday evening, you face a critical decision: **Where should each truck be positioned on Saturday to maximize revenue?**

This isn't a simple location selection problem. Each truck has the operational capability to **relocate once during the day**, creating a four-location optimization challenge:

| Truck | Morning Position (7 AM – 12 PM) | Afternoon Position (2 PM – 8 PM) |
|-------|--------------------------------|----------------------------------|
| **Truck A** | Location ? | Location ? |
| **Truck B** | Location ? | Location ? |

The Thursday deadline gives you Friday for crew coordination, supply runs, and logistics planning. Your partner expects clear recommendations backed by data-driven justification.

---

## The Menu Structure

Capitol Slice operates with distinct menu offerings by time of day, which influences location strategy:

### Breakfast Menu (7 AM – 12 PM)
Premium breakfast pizza slices: eggs, bacon, chorizo, vegetable options  
**Price range:** $5 – $7 per slice

### Signature Menu (11 AM – 9 PM)  
Classic and specialty slices: Margherita, pepperoni, white pizza, seasonal offerings  
**Price range:** $5 – $7 per slice

This menu split means morning locations should favor breakfast-seeking demographics (farmers markets, metro commuters, weekend brunch crowds), while afternoon positioning targets event attendees and general foot traffic.

---

## The 10 Potential Locations

Your operation has permits for 10 strategically selected positions across DC. Each location has distinct characteristics that make it optimal under certain conditions and suboptimal under others.

**See companion document: `capitol-slice-site-analysis.md`** for detailed breakdown of each location including strengths, weaknesses, and optimal conditions.

| # | Location | Category | Key Characteristic |
|---|----------|----------|-------------------|
| 1 | Eastern Market | Market District | Weekend flea market, morning-heavy |
| 2 | Dupont Circle | Metro/Urban Hub | Farmers market, constant foot traffic |
| 3 | National Mall | Tourist/Monument | Highest volume, weather-dependent |
| 4 | Georgetown Waterfront | Waterfront/Upscale | Scenic destination, weather-dependent |
| 5 | U Street Corridor | Arts/Music | Evening-focused, concert proximity |
| 6 | Convention Center | Convention/Business | High-value when events scheduled, dead otherwise |
| 7 | Capital One Arena | Sports/Entertainment | Game-day dependent, weather-independent |
| 8 | Columbia Heights | Residential | Neighborhood backup, lower risk |
| 9 | H Street Corridor | Arts/Festival | Festival-driven, growing destination |
| 10 | Navy Yard / The Wharf | Waterfront/Sports | Nationals games, waterfront dining |

---

## Decision Factors

Your optimization must account for three dynamic variables that change weekly:

### Factor 1: Weather Forecast

Weather impacts your operation in multiple ways:

**Direct Effects:**
- Precipitation probability affects customer willingness to wait outdoors
- Temperature extremes reduce foot traffic
- Wind conditions matter for outdoor setup

**Indirect Effects:**
- Bad weather makes indoor events MORE attractive (sports games, conventions)
- Good weather makes outdoor locations MORE attractive (waterfront, National Mall)
- Weather affects competing food trucks' decisions

**Data Requirements:**
- 7-day forecast with hourly granularity
- Precipitation probability thresholds
- Temperature and wind speed

---

### Factor 2: Events and Foot Traffic

DC's event calendar directly drives location value:

**Sports Schedules:**
- Nationals (MLB) – 41,000 capacity, afternoon/evening starts
- Wizards (NBA) – 18,000 capacity, evening/afternoon starts  
- Mystics (WNBA) – 18,000 capacity, variable scheduling
- Capitals (NHL) – 18,000 capacity, evening starts
- DC United (MLS) – Audi Field, 20,000 capacity

**Recurring Markets:**
- Eastern Market weekend flea market
- Dupont Circle farmers market
- Various neighborhood markets

**Festivals and Special Events:**
- H Street Festival
- National Mall events (rallies, concerts, celebrations)
- Convention Center bookings
- Cultural festivals across neighborhoods

**Event Classification Matters:**
- **Indoor events** become MORE valuable in bad weather
- **Outdoor events** become LESS valuable in bad weather
- **Timed events** (games, concerts) create predictable traffic windows
- **All-day events** (markets, festivals) allow flexible positioning

---

### Factor 3: Competitive Positioning

Other food trucks are solving the same optimization problem:

**Competition Sources:**
- Direct pizza competitors (rare in DC mobile food scene)
- Indirect competitors (tacos, sandwiches, Asian cuisine)
- Restaurant spillover effects

**Intelligence Gathering:**
- Food trucks announce locations via social media (Instagram, Twitter/X)
- Aggregator sites track truck positions
- Historical patterns reveal competitor tendencies

**Strategic Implications:**
- Two pizza trucks at same location = split market
- Indirect competition matters less than direct
- Some locations attract food truck clusters
- First-mover advantage at premium spots

---

## The Optimization Challenge

Your weekly Thursday evening deliverable must answer the following questions in a structured memo to your partner that answers the following questions.

The memo cannot exceed two pages, including all text, diagrams, charts, etc. and should be easily understandable by team members with no formal data training

1. **Where should Truck A start Saturday morning?**
2. **Where should Truck B start Saturday morning?**
3. **Should either truck relocate in the afternoon? If so, where?**
4. **What's the expected revenue impact of this configuration?**
5. **What risks exist in this plan, and what's the backup if conditions change?**

### Constraints to Consider:

**Relocation Logistics:**
- Moving a truck requires ~45-60 minutes (teardown, transit, setup)
- Lost revenue during movement window
- Crew fatigue from setup/teardown cycles
- Fuel and logistics costs

**Information Timing:**
- Weather forecasts improve closer to Saturday
- Event schedules are known in advance
- Competitor positions may not be announced until Friday/Saturday morning

**Operational Realities:**
- Trucks cannot be at same location (cannibalization)
- Some locations require reservations/permits
- Crew preferences and experience matter
- Supply chain (ingredient prep) must align with menu expectations

---

## Your Assignment

Build an automated decision support system that:

1. **Ingests weekly data** on weather, events, and competition
2. **Scores each location** based on current conditions
3. **Recommends optimal positioning** for both trucks across both time windows
4. **Provides justification** a business partner can understand and trust
5. **Generates the specified deliverable** by Thursday evening each week

The solution should be repeatable, data-driven, and produce actionable recommendations with minimal manual intervention.

---

## Data Sources Reference

| Data Need | Possible Data Sources |
|-----------|-------------------|
| Weather forecast | National Weather Service API (NOAA), OpenWeather |
| Sports schedules | ESPN API, team websites, MLB/NBA/NHL/WNBA APIs |
| Events | Eventbrite API, washington.org, DC.gov calendar |
| Competitor positions | Social media (Instagram, Twitter/X), food truck aggregators |
| Historical performance | Internal tracking (build over time) |

---

## Solution Objectives

Your solution should meet the following criteria:

- **Data integration**: Successfully pulling from multiple sources
- **Scoring logic**: Defensible weighting of factors
- **Automation**: Minimal manual steps required weekly
- **Clarity**: Partner can understand recommendations without technical background
- **Adaptability**: System handles missing data, edge cases, unusual weeks

---

*This case study is designed to simulate real-world data analysis challenges: multiple data sources, competing objectives, uncertainty, and the need to communicate technical recommendations to non-technical stakeholders.*

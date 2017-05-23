# fast-trips_dwell_time_model
Develop dwell time model for King County and San Francisco

## Content
This repository suggests dwell time model specifications for bus systems in the Puget Sound Region (King County Metro) and the San Francisco Bay Area (Muni, operated by the San Francisco Municipal Transportation Agency, SFMTA). 
For other bus transit operators and non-bus transit modes, an inferred dwell time specification is suggested based on the Transit Capacity and Quality of Service Manual (TCQSM)


Model specification recommendations balance estimation robustness and reasonableness while retaining desired policy levers. 
San Francisco’s suggested policy levers include standard versus articulated buses, low-floor vehicles, and all-door boarding policy.  
In the Puget Sound, the recommended policy variables include off-board fare payment and vehicle type.


## Input data
This analysis uses data from both SF Muni and KC Metro to capture the impact of vehicle and stop-based amenities on bus dwell times, while isolating geographically-biased influences. The data used includes:
* King County Metro Spring 2015 APC: six days, 334,254 records
* San Francisco Muni Spring 2015 APC: six days, 266,817 records
* King County Metro Spring 2014 APC: one day, 47,498 records
* San Francisco Muni Fall 2012 APC: one day, 94,460 records


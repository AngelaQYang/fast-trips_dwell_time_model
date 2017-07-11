# Fast-Trips Dwell Time Model

## Content
Dwell time model explores and suggests transit vehicle dwell time functions, for use in the Puget Sound and San Francisco Bay Area implementations of Fast-Trips (https://github.com/MetropolitanTransportationCommission/fast-trips). 
* Project Website: http://fast-trips.mtc.ca.gov/
* Full Technical Documentation (API): http://metropolitantransportationcommission.github.io/fast-trips/


This repository suggests dwell time model specifications for bus systems in the Puget Sound Region (King County Metro) and the San Francisco Bay Area (Muni, operated by the San Francisco Municipal Transportation Agency, SFMTA). 
For other bus transit operators and non-bus transit modes, an inferred dwell time specification is suggested based on the Transit Capacity and Quality of Service Manual (TCQSM).


Model specification recommendations balance estimation robustness and reasonableness while retaining desired policy levers. 
* San Francisco’s suggested policy levers include standard versus articulated buses, low-floor vehicles, and all-door boarding policy.  
* In the Puget Sound, the recommended policy variables include off-board fare payment and vehicle type.


## Input
This analysis uses data from both SF Muni and KC Metro to capture the impact of vehicle and stop-based amenities on bus dwell times, while isolating geographically-biased influences. The data used includes:
* King County Metro Spring 2015 APC: six days, 334,254 records
* San Francisco Muni Spring 2015 APC: six days, 266,817 records
* King County Metro Spring 2014 APC: one day, 47,498 records
* San Francisco Muni Fall 2012 APC: one day, 94,460 records

## Published Data 
We have published the data on Box for internal use here: https://app.box.com/files/0/f/11594143211/Dwell_Time_Model. More is coming, stay tuned. 

## TCQSM
The Transit Capacity and Quality of Service Manual (TCQSM) (http://www.trb.org/Main/Blurbs/169437.aspx) provides guidance on transit capacity and quality of service issues and the factors influencing both.  The manual includes quantitative techniques for calculating the capacity and other operational characteristics of bus, rail, demand-responsive, and ferry transit services, as well as transit stops, stations, and terminals. Regarding dwell time, TCQSM presents three methods to estimate the dwell time: field measurement, default values, and calculation.

The TRB website above provides an Excel version of the TCQSM calculations which we have included in this repository in the folder: \TCQSM_comp\build_TCQSM\tcqsm_demo_excel.  In order to understand how factors such as vehicle type and fare policy influence passenger flow time, and to use the TCQSM model with our observed dataset, a IPython notebook (available here: \TCQSM_comp\build_TCQSM\TCQSM_2.0.ipynb) was scripted to show the TCQSM calculation flow. You can play with the model by changing different inputs within the code.  


Hope this repository will help you get to know the dwell time model structure easier.

## References
SFMTA (2012) All-Door Boarding Evaluation Final Report. https://www.sfmta.com/sites/default/files/agendaitems/2014/12-2-14%20Item%2014%20All%20Door%20Boarding%20Report.pdf 
 
Lisa Zorn, Elizabeth Sall, and Daniel Wu (2012) Incorporating crowding into the San Francisco activity-based travel model. Transportation 39(4): 755-771. http://link.springer.com/article/10.1007%2Fs11116-012-9405-x
 
Transit Capacity and Quality of Service Manual, Third Edition. http://www.trb.org/Main/Blurbs/169437.aspx 
 
Kenneth J. Dueker, Thomas J. Kimpel, James G. Strathman (2004) Determinants of Bus Dwell Time. Journal of Public Transportation, Vol. 7, No. 1, 2004. http://www.nctr.usf.edu/jpt/pdf/JPT%207-1%20Dueker.pdf 
 
Grant Fletcher and Ahmed El-Geneidy (2013) Efforts on Fare Payment Types and Crowding on Dwell Times. Journal of the Transportation Research Board, No. 2351, 2013, pp. 124–132.  http://tram.mcgill.ca/Research/Publications/Translink_Dwell_Analysis.pdf 

# NAP-State

This repository is an experimental table for national access point tracking per country based on EU/1926/2017 (https://eur-lex.europa.eu/legal-content/EN/TXT/PDF/?uri=CELEX:32017R1926&from=DE) 

## The NAPs
https://github.com/ue71603/NAP-State/blob/main/nap/nap.md


## Data provision
One part is providing the necessary data as datasets. We distinguish:
* Basic data
* Timetables (and time table analogons)
* Realtime data
* Others

###Timetables and real time data
Timetables and the like are often provided in different formats. The regulation names only NeTEx and Siri and the like. Therefore only those are considered. It may be that we will have to extend this later.

|Country|URL|NeTEx timetable|Fares|Siri PT|Siri ET|Siri FM | Siri VM|Siri SX|
|--|--|--|--|--|--|--|--|--|
|Switzerland|https://opentransportdata.swiss/de/|Experimental|-|Soon|Soon|-|-|Soon|
|Austria|<ul><li>OeBB: https://data.oebb.at/#default/support</li><li>Arge-öVV</li></ul>|?|?|?|?|?|?|?|

##Types of the static travel data

### Trip planner service (level 1)
|Country|URL|Location search|Trip plans|Location search (accessnodes)|Trip plan computation|Trip plan computation (road)|Location search (demand-responsive modes)|Information service|
|--|--|--|--|--|--|--|--|--|
|Switzerland|xxx|POI missing|yes|?|Limitation in (v),(viii),(ix),(x), (ii) topology missing|done, but not perfect|Refuling missing, secure bike parking missing, not in production yet|?|


### Trip planner service (level 2)
|Country|URL|Location search (demand-responsive modes)|Information service|Trip plans, auxiliary information, availability check|
|--|--|--|--|--|
|Switzerland|xxx|Refuling missing, secure bike parking missing, not in production yet|?|?|


### Trip planner service (level 3)
|Country|URL|Detailed common standard and special fare query (all scheduled modes)|Information service (all modes)|Trip plans|Trip computation|
|--|--|--|--|--|--|
|Switzerland|xxx|?|?|?|?|

## Types of the dnamic travel and traffic data

### Level of service 1
|Country|URL|Passing times, trip plans and auxiliary information|
|--|--|--|
|Switzerlan|xxx|?|

### Level of service 2
|Country|URL|Passing times, trip plans and auxiliary information (all modes)|Information service|Availability check|
|--|--|--|--|--|
|Switzerlan|xxx|?|?|?|

### Level of service 3
|Country|URL|Trip plans|
|--|--|--|
|Switzerlan|xxx|no, no realtime road data|

# NAP-State

This repository is an experimental table for national access point tracking per country based on EU/1926/2017 (https://eur-lex.europa.eu/legal-content/EN/TXT/PDF/?uri=CELEX:32017R1926&from=DE) 

## Methdology
https://github.com/ue71603/NAP-State/blob/main/methodology.md

## The NAPs
https://github.com/ue71603/NAP-State/blob/main/nap/nap.md


## Data provision
One part is providing the necessary data as datasets. We distinguish:
* Basic data
* Timetables (and time table analogons)
* Realtime data
* Others

### Basic data
Basic data often is not provided directly by the NAP, but by other entities. We had to take this into account.

#### Datasets
|Country|Address information|Topographic Places|POI|Petrol stations |Charing stations |Park&Ride stations |Bike-Sharing stations |Car-Sharing-Stations|safe bike  parking|Road network|Detailed cycle network|Environmental impact calculation|Power usage for vehicles|
|--|--|--|--|--|--|--|--|--|--|--|--|--|--|
|Switzerland|?|?|?|?|?|?|?|?|?|?|?|?|?|
|Switzerland|?|?|?|?|?|?|?|?|?|?|?|?|?|

Public transport
|Country|Routes|Calendar&DayTypes|stops|Geometry / details stops|Operators|Timetables|Interchange time|Guaranteed interchange|Operating hours|Equipment at stops|Vehicle (types|routing within stops|Assistance|
|--|--|--|--|--|--|--|--|--|--|--|--|--|--|
|Switzerland|n/a|NeTEx|NeTEx|TSI PRM/ <br>EPIAP missing <br> or use OSM|NeTEx|NeTEx|NeTEx|NeTEx (spotty)|NeTEx|missing|missing|missing (use OSM)|missing|


Information services
|Country|Order channels|Base and normal tarrifs line traffic|Vehicle equipments|Maut channels|Directory service for ordering|Parking fees|
|--|--|--|--|--|--|--|
|Switzerland|missing|missing|partly NeTEx, party missing|missing|missing|missing|

#### Used in Distributed trip planner

### Timetables and real time data
Timetables and the like are often provided in different formats. The regulation names only NeTEx and Siri and the like. Therefore only those are considered. It may be that we will have to extend this later.

|Country|URL|NeTEx timetable|Fares|Siri PT|Siri ET|Siri FM | Siri VM|Siri SX|DATEX II actual road times|DATEX II blocked roads|
|--|--|--|--|--|--|--|--|--|--|--|
|Switzerland|https://opentransportdata.swiss/de/|Experimental <br> Missing: Routes, POI, vechile types|not available|soon|soon|not available|notavailable|soon, but only some operators|?|
|Austria|<ul><li>OeBB: https://data.oebb.at/#default/support</li><li>Arge-öVV</li></ul>|?|?|?|?|?|?|?|?|?|

# API for trip planning

## Types of the static travel data

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
|Switzerland|xxx|?|

### Level of service 2
|Country|URL|Passing times, trip plans and auxiliary information (all modes)|Information service|Availability check|
|--|--|--|--|--|
|Switzerland|xxx|?|?|?|

### Level of service 3
|Country|URL|Trip plans|
|--|--|--|
|Switzerland|xxx|no, no realtime road data|

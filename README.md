<img src="misc/REPR.svg" alt="REPR-logo">

# Residential Energy Performance Rating (REPR)
## Residential Energy Performance Scoring
### :question: What is Residential Energy Performance Score
Inspired by Energy Star's [Energy Performance Score](https://portfoliomanager.energystar.gov/pdf/reference/ENERGY%20STAR%20Score.pdf) for public and commercial buildings, our team developed the Residence Energy Performance Scoring, a 1-100 score providing a quantitative comparison between the energy efficiencies of residential homes.

The score aims to provide a benchmark based on similar house attributes and energy usages. The score is calculated by comparing the home's energy usage to its peers with statistical methods to provide a fair score regardless of home-specific factors.

To present use cases of the scoring system, our team developed Residential Energy Performance Rating System (REPR), a software application providing various features based on the scoring system.

### :heavy_plus_sign: How the 1-100 Score is calculated?
For convenience, we refer to these factors as type 1 variables and any other factors that influence the energy efficiency as type 2 variables. 

The estimated energy usages are used to calculate the energy efficiency ratio with the actual energy usage. 
```
 Energy Efficiency Ratio = Actual EUI / Expected EUI
```
This ratio represents the relative measure of how energy-efficient the home is by comparing the actual energy usage to expected energy usage given different building or geographical factors discussed above(type 1). When the ratio is high, the residence building is less energy efficient, and vice versa. 

The energy efficiency ratio is compared with multiple peers with similar home attributes by fitting a probability distribution. The peers are found using statistical clustering analysis with the type 1 variables. To view detail example of how to calculate the score, please see the [IPython notebook]().

### :open_file_folder: Data
To build tranditional 1-100 ENERGY STAR rating, [CBECS(US)](https://www.eia.gov/consumption/commercial/) and [SCIEU(Canada)](https://oee.nrcan.gc.ca/corporate/statistics/neud/dpa/menus/scieu/2014/tables.cfm) datasets were used. These data are from government surveys to understand energy usage in commercial and institutional buildings. Similarly, the government also did [RECS(US)](https://www.eia.gov/consumption/residential/) and [SECMURB(Canada)](https://oee.nrcan.gc.ca/corporate/statistics/neud/dpa/menus/murb/2018/tables.cfm) to sample energy usage in residential buildings. We performed analysis on RECS to build our score system

## Residential Energy Performance Rating (REPR)
The REPR is a web application developed to demonstrate different use-cases of the Residential Energy Performance Scoring system. The application includes a dashboard for 
* Homeowners who want to evaluate the energy efficiency of their home and receive general recommendations to improve the score. 
* Analysts want to gain further insights into the driving factors of residential energy efficiency. 

##
<img src="misc/user-dashboard.png" alt="user-dashboard"/>


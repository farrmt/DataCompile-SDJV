---
output:
  pdf_document: default
  html_document: default
---

# PSSS {#PSSS5}



<img src="images/PSSS.PNG" width="700px" style="display: block; margin: auto;" />

## Quick Data Overview {#PSSS5.1}

| Data        | Puget Sound Seabird Survey (PSSS)                                    |
|-------------------------|----------------------------------------------|
| Owner       | Seattle Audubon/ Puget Sound Bird Observatory                        |
| Status      | Active                                                               |
| Years       | ?? - present                                                         |
| Seasons     | Monthly survey, with a winter focus from Oct - April                 |
| Sampling    | Coastal surveys at designated points                                 |
| Data Access | Available by contacting data owner                                   |
| Contact     | [joshm\@seattleaudubon.org](mailto:joshm@seattleaudubon.org){.email} |

[PSSS Website](https://seattleaudubon.org/wp-content/uploads/2021/01/PSSS_Protocol_2014-15.pdf).

## Data Collection Protocol {#PSSS5.2}

PSSS protocol can be found online [here](https://www.birdscanada.org/bird-science/british-columbia-coastal-waterbird-survey/bccws_resources).

In short, surveys have been conducted by volunteers using a standardized protocol and data collection [sheets](https://seattleaudubon.org/wp-content/uploads/2021/09/PSSS-Datasheet.pdf). Shore-based counts are completed monthly on the first Saturday of each month from October to April. Surveys are complete within approximately 2 hour of high tide to maximize the opportunity for close observation. Surveys are a minimum of 15 minutes and a maximum of 30 minutes per site. All waterbirds observed to a distance of 300 m from the high tide line are counted, except those that fly through without stopping. For large flocks, surveys estimate both the min, max, and best estimate. Surveyors are required to attend a short training session with the Seattle Audubon staff prior to their first survey. Data are entered through a customized online data entry system available [here](http://seabirdsurvey.org/seabirdsurvey/).

## Avian Data Collected {#PSSS5.3}

Total observation counts of each waterbird species seen during a point survey are recorded for each monthly, including bearing, distance, and sex ratio. Raptor number and species are recorded separately from the other waterbird species. The dataset is not zero-filled.

Taxonomic Authority =

## Auxiliary Data Collected {#PSSS5.4}

-   Observer information: observer name

-   Survey Information: time observation started, time observation ended

-   Survey Condition: weather, precipitation, sea state, tide movement, visibility, human activity, raptor activity (all categorical)

## Data Access, Permission, and Format {#PSSS5.5}

At the time of writing, the data were only accessible by reaching out to the Seattle Audubon directly and filling out a data share agreement. The data will be sent as a .xslx flat file which will be suitable for processing.

## Data Use Considerations {#PSSS5.6}

The data are collected using a standardize protocol, by trained citizen-science volunteers. This standardization is a strength of this datasets for making inferences about coastal waterbirds in the US Salish Sea.

Since surveyors gathers information on distance and direction, estimates of bird density through distance sampling is possible. Specifically, detection of any species declines with the distance from the observer: poor sighting conditions, quality of observing equipment, and observer inexperience all contribute to declining detection likelihood as distance increases. Distance sampling provides a robust approach to estimating density and allow for calculation of less biased density estimates.

The repeated sampling design of the PSSS makes this dataset suitable for an occupancy modelling framework, in which the probability of detection can be modeled alongside occupancy. Auxiliary data collected during each survey are suitable for the detection process of the model.

Measures of effort are innate to the dataset. Survey duration can be used to make effort correction to counts.

*There is spatial inbalance in the sampling design?* Since this survey is shore-based, there will be a species sampling bias. Specifically, birds that use near shore habitats will be detected and counted more often than birds which use offshore habitats. This dataset may therefore be less suitable for modelling sea bird habitat use, for example.

This PSSS survey was designed to be similar to the BCCWS, with some notable differences:

| BCCWS                     | PSSS                      |
|---------------------------|---------------------------|
| Survey the second Sunday  | Survey the first Saturday |
| Sept-April                | Oct-April                 |
| 1km count distance        | 300m count distance       |
| Survey route              | Single point              |

## Data Processing {#PSSS5.7}

Once the full dataset has been received, save it in the `Data` folder found in this R project directory. You will find a sample dataframe has already been saved for the purposes of this example.
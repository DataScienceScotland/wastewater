
## Scottish Government Covid-19 Modelling

### Wastewater

Levels of Wastewater SARS-Cov-2 RNA are collected at a large number of
sites around Scotland and adjusted for population and local changes in
intake flow rate. These estimates are provided by [Biomathematics &
Statistics Scotland (BioSS)](https://www.bioss.ac.uk/).

Samples from Waste Water Treatment Works (WWTW) in Scotland have been
collected by Scottish Water and analysed by the Scottish Environment
Protection Agency (SEPA) to detect fragments of SARS-Cov-2 virus RNA in
wastewater. This is reported from lab analysis as gene copies per litre.

Raw measurements of this concentration of wastewater RNA are affected by
both the size of the catchment area at each waterworks (and hence the
population served), as well as the amount of flow into the works (with
high volumes of fluid flow diluting RNA values).

BioSS normalise values by flow and population using methodology detailed
in the following paper:
<https://www.protocols.io/view/data-normalisation-of-rt-qpcr-data-for-detection-o-5qpvoby8bl4o/v1>.
An external peer review of this work is currently underway.

The flow values derive from one of three estimates depending on data
availability:

  - Direct flow: When measurements of flow are available, we multiply
    the raw RNA measurement by the daily flow total, and divide by the
    population served at each site, to produce a daily value of RNA
    copies per person.

  - Ammonia-based estimate: In some cases (especially with the most
    recent data), flow measurements are unavailable; if however
    measurements of ammonia concentration are available, they can be
    used to estimate flow via a statistical model.

  - Interpolated estimate: : When both flow and ammonia measurements are
    unavailable, we estimate flow and ammonia from a model using
    historical data and other sites. This involves that site’s average
    difference from other sites, and the national trend over time of
    ammonia concentrations (assumed nonlinear but smooth). When a site
    has no associated flow data at all, a prediction is calculated based
    on the population characteristics of the site.

### Other Covid-19 Modelling

This model is one of a
[series](https://github.com/search?q=topic%3Ac19-modelling+org%3ADataScienceScotland+fork%3Atrue)
used by the Scottish Government during the pandemic to model the spread
and levels of Covid-19 in Scotland. Many of the results of these models
have been published in the [Modelling the
Epidemic](https://www.gov.scot/collections/coronavirus-covid-19-modelling-the-epidemic/)
series of reports.

If you have any questions regarding the contents of this repository,
please contact <sgcentralanalysisdivision@gov.scot>.

### Licence

This repository is available under the [Open Government Licence
v3.0](http://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/).

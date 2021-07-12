# Covid-19_Bharat_records

<br>This repository parses & archives COVID-19 test positivity percent for Indian districts and states. The test positivity is the fraction of Covid tests that are positive.</br>

<br>From 10th May onwards, the Indian Ministry of Health has been uploading a daily Excel file that reports the weekly average COVID-19 test positivity for Indian districts with a test positivity ≥ 10%. From 26th May onwards, this data set has been expanded to include data from almost all districts.</br>

<br>This repository automatically fetches the daily government data update, parses the data and appends it to a CSV file, and archives the government data file.</br>

<br>We also calculate the test positivity for Indian states & union territories using data collected by covid19india.org as follows: test positivity (7 day average) = new confirmed cases in the past week / tests conducted in the past week. Note that there may be some discrepancies between states depending on whether they report the number of samples tested or the number of people tested.</br>

# Data Sources
<br>*District Data: [Indian Ministry of Health](https://www.mohfw.gov.in/)</br>
<br>*State Data: [covid19india.org](https://api.covid19india.org/)</br>

#Data Files
*The archive folder contains an archive of the daily government Excel files with test positivity data for districts
*districtdata.csv contains time-series test positivity data for districts
*statedata.csv contains time-series test positivity data, weekly confirmed cases, and weekly tests for states & union territories
<br> The date is in ISO format i.e. YYYY-MM-DD. Test positivity is calculated as a 1 week average for the 7 days prior to the date on which the data is reported. For example, the test positivity reported on June 8 is based on the new cases / tests on June 1 through June 7.</br>

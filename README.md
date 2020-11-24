# Coronavirus statistics in Finland.

Web-site: [https://sufflavus.github.io/coronavirus-in-finland](https://sufflavus.github.io/coronavirus-in-finland)

Supported languages: English, Russian

Source code: [On Bitbucket](https://bitbucket.org/Sufflava/coronavirus-statistics-in-finland/src/master/web-site/)

Data: [Saved files](https://bitbucket.org/Sufflava/coronavirus-statistics-in-finland/src/master/data/)

All the numbers, that are shown on this website, are taken from the official THL's website (National Institute for Health and Welfare of Finland) and offician THL's API.

## Statistics that is shown
- Current situation - summed up numbers (for the whole country, for all the time)
- Chart with daily dynamic (for the whole country)
- Current hostpitalisations - number of people that are currently hospitalised (for the whole country)
- Statistics by age
- Statistics by sex
- Chart with daily number of cases devided by regions

![site_screenshot_1](https://bitbucket.org/Sufflava/coronavirus-statistics-in-finland/raw/51d4d70c1b476bbd5ca38e6d07041ec60310c708/images/site_screenshot_1.png)

![site_screenshot_2](https://bitbucket.org/Sufflava/coronavirus-statistics-in-finland/raw/51d4d70c1b476bbd5ca38e6d07041ec60310c708/images/site_screenshot_2.png)

![site_screenshot_3](https://bitbucket.org/Sufflava/coronavirus-statistics-in-finland/raw/51d4d70c1b476bbd5ca38e6d07041ec60310c708/images/site_screenshot_3.png)

![site_screenshot_4](https://bitbucket.org/Sufflava/coronavirus-statistics-in-finland/raw/51d4d70c1b476bbd5ca38e6d07041ec60310c708/images/site_screenshot_4.png)

![site_screenshot_5](https://bitbucket.org/Sufflava/coronavirus-statistics-in-finland/raw/899cedff04845dff276de75dddbcbeabed3e0fec/images/site_screenshot_5.png)

![site_screenshot_6](https://bitbucket.org/Sufflava/coronavirus-statistics-in-finland/raw/899cedff04845dff276de75dddbcbeabed3e0fec/images/site_screenshot_6.png)

## Statistics that will be added soon
- Map view

## API request calls and resources that were used for getting data:
- daily country wide statistics in English (number of tests, number of positive cases, number of deaths)

[https://sampo.thl.fi/pivot/prod/en/epirapo/covid19case/fact_epirapo_covid19case.json?column=dateweek2020010120201231-443702L&column=measure-141082](https://sampo.thl.fi/pivot/prod/en/epirapo/covid19case/fact_epirapo_covid19case.json?column=dateweek2020010120201231-443702L&column=measure-141082)

- total numbers for current date are taken from weekly statistics

[https://sampo.thl.fi/pivot/prod/en/epirapo/covid19case/fact_epirapo_covid19case.json?row=dateweek2020010120201231-443686&column=measure-141082](https://sampo.thl.fi/pivot/prod/en/epirapo/covid19case/fact_epirapo_covid19case.json?row=dateweek2020010120201231-443686&column=measure-141082)

- number of hostpitalisations are taken from THL's web site

[https://thl.fi/en/web/infectious-diseases-and-vaccinations/what-s-new/coronavirus-covid-19-latest-updates/situation-update-on-coronavirus](https://thl.fi/en/web/infectious-diseases-and-vaccinations/what-s-new/coronavirus-covid-19-latest-updates/situation-update-on-coronavirus)

- statistics by region (coming soon)
- statistics by age

Number of positive cases devided by age:

[https://sampo.thl.fi/pivot/prod/en/epirapo/covid19case/fact_epirapo_covid19case.json?column=ttr10yage-444309](https://sampo.thl.fi/pivot/prod/en/epirapo/covid19case/fact_epirapo_covid19case.json?column=ttr10yage-444309)

Number of deaths devided by age:

[https://sampo.thl.fi/pivot/prod/en/epirapo/covid19case/fact_epirapo_covid19case.json?column=measure-492118&column=ttr10yage-444309](https://sampo.thl.fi/pivot/prod/en/epirapo/covid19case/fact_epirapo_covid19case.json?column=measure-492118&column=ttr10yage-444309)

- statistics by sex

Number of positive cases devided by sex:

[https://sampo.thl.fi/pivot/prod/en/epirapo/covid19case/fact_epirapo_covid19case.json?column=sex-444328](https://sampo.thl.fi/pivot/prod/en/epirapo/covid19case/fact_epirapo_covid19case.json?column=sex-444328)

Number of deaths devided by sex:

[https://sampo.thl.fi/pivot/prod/en/epirapo/covid19case/fact_epirapo_covid19case.json?column=measure-492118&column=sex-444328](https://sampo.thl.fi/pivot/prod/en/epirapo/covid19case/fact_epirapo_covid19case.json?column=measure-492118&column=sex-444328)

## Statistics that has not been found yet
- Daily dynamic of hospitalisations, country wide and devided by region (currently, only today's numbers are available)
- Daily total number of deaths (not only coronavirus), country wide and devided by region
- Daily number of tests that are done devided by age and sex
- Daily number of tests and deaths devided by region (currently only country wide numbers are available)

## Used libraries:
- [JSON-stat Javascript Toolkit](https://www.npmjs.com/package/jsonstat-toolkit)
- [Recharts](https://recharts.org/en-US/)
- [schemecolor](https://www.schemecolor.com/stunning-pie-chart-color-scheme.php)
- [momentjs](https://momentjs.com/)
- [React](https://reactjs.org/)
- [Redux](https://redux.js.org/)
- [react localize redux](https://ryandrewjohnson.github.io/react-localize-redux-docs/)

## Contributors
 - [Lasicaine](https://github.com/Lasicaine) (Design & usability)

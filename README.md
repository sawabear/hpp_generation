# hpp_generation
Hydroelectric generation prediction.

# Some details
First, we download data from IRI (International Research Institute for Climate and Society: IRIhttps://iri.columbia.edu). We use their weather forecast (precipitation forecast). The open data only has a forecast for 6 months, so we use the prophet for the forecast for the next period (3 years).

In the second step, I use different information about hydroelectric power station and IRI precipitation for teaching catboost. 

At the third stage, we use the "balanced method" to adjust the forecast of various indicators of the object.

In final, we predict hydro power plant generation value per month.

This information helps predict prices. As a result, this allows us to estimate the future income and expenses of the company.

# Use
1. catboost
2. pandas
3. prophet
4. pyodbc

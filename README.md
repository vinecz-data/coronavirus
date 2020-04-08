# COVID-19 VIRUS GLOBAL REPORT

Technology

Database Host: Snowflake
<br>
Integrator Tool: Pentaho Data Intration
<br>
Dashboard Tool: Microsoft Power BI


[Open Dashboad Here](https://app.powerbi.com/view?r=eyJrIjoiNTFmNzExYzktN2QyNi00ZGNhLTg1MjQtYTUyOWIyMGYzOGI2IiwidCI6IjE1M2U3N2E0LWMyOWQtNGYyZS04ODU3LWU0MDU5M2YxNjkzMCJ9)

Guide of files:

<b>main_job.kjb</b> - Pentaho main JOB, that orquestrate all flow. <br>
<b>snowflake_corona.ktr</b> - Pentaho Transformation that download the JSON hosted in https://pomber.github.io/covid19/timeseries.json and generate a file in my local directory. <br>
<b>snowflake.sh</b> - Shell script that connects in Snowflake via snowsql and do the PUT command to load the .JSON file into a internal stage called @DW_SPOT_STAGE.

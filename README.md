There are two notebooks in this repository.

The notebook nz_crime_locations.ipynb processes data downloaded from policedata.nz (https://www.police.govt.nz/about-us/publications-statistics/data-and-statistics/policedatanz). The output of this code is then used as an input to the Power BI dashboard linked to below:
https://app.powerbi.com/view?r=eyJrIjoiZWJjODVkMmUtNjYzOC00ZjA4LWExOWItNjU5MDIxZmY2NTI0IiwidCI6Ijg0ODgwZWExLTdkNTktNDRmYS1hMWYzLWM0YzdhYjZiODUxZiJ9
This visualises the location of all recorded crimes across NZ over the period from APR2022 to MAR2023.

The notebook w1c_obtain_make_model_age_class_type.ipynb basically takes a set of Vehicle Identification Numbers (VINs) and attempts to find make, model, vehicle type, vehicle class, year and fuel type information from the VEEEL and NZTA APIs. The code works by first mathcing all vehicles to a reference library. If the vehicle is not found within the library then the (free) VEEEL API is called to retrieve the required information. If the required information about the vehicle is still not found, the vehicle is passed to the NZTA API at an incurred cost. This code is just one program in a sequence of programs that powers the Optifleet Scope3 Emissions dashboard designed to estimate CO2e emissions resulting from the movements of an organisation's fleet. A link to a demo version of this dashboard is provided below:
https://app.powerbi.com/view?r=eyJrIjoiZGI1MTlkOTQtMzJhOC00ZWQxLWEwNDMtM2MxYzMwMGRiMjIxIiwidCI6Ijg0ODgwZWExLTdkNTktNDRmYS1hMWYzLWM0YzdhYjZiODUxZiJ9

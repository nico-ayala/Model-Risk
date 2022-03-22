# Using aggregate statistical data, a method based on linear models to estimate COVID-19 Relative Risk. The case of Catalonia .
## Abstract text.

1. Introduction. SARS-CoV-2 is a new type of coronavirus that causes COVID-19. It is affecting the entire planet. Despite the widespread use of ecologic analysis in epidemiologic research and health planning, health scientists and practitioners have given little attention to the methodological aspects of this approach. The study of risk factors linked to the COVID-19 pandemic is one of the most current and exciting topics for epidemiologists. These risks in many cases are unknown. This research covers the study of risk factors in the case of COVID-19 and proposes the use of an ecologic method known to epidemiologists in the case of aggregated data. 
2. Objective: The present study aims to compute a model that allows to easily calculate the risk of infection in different types of populations, using aggregated data to approximate the individual risk of COVID-19 transmission by a person. 
3. Materials and methods: The case of Catalonia, in Spain, is presented as an example, as it is one of the areas where the incidence of the virus among the population is being higher. The proposed method is known as an ecological study and is based on the statistical regression model between the incidence (or variable that represents it) and the risk factors but using aggregated data and obtaining a risk ratio (RR). It is intended to utilize a model of the incidence as a function of the mobility, density of population, etc. to determine the relative ecological risk of the population and of the person contracting COVID-19, using ecological epidemiology methods. 
4. Results: The results obtained have made it possible to find the risk of contracting COVID-19 concerning risk factors for low family income (RR=1.157491), more mobility (RR=1.065475), and high density of population (1.00002). 
5. Conclusions: This method could be used to design an app that predicts how the risk will evolve and calculate the risk of contagion in one area or another to take action. The calculated RR can help us to understand how the variables become risks or protective factors at an ecological level (understanding aggregate data).

**Keywords: COVID-19, outbreak, epidemic dynamics, modelling, relative risk.**

## Database. 
The data used to feed the model was obtained from different public sources such as IDESCAT (Institute of Statistics of Catalonia): 
https://www.idescat.cat/pub/?id=aec&n=250&lang=es ; https://www.idescat.cat/emex/?id=080193#h40000000

Generalitat of Catalonia (Catalonia Government):http://aquas.gencat.cat/ca/actualitat/ultimes-dades-coronavirus/mapa-per-abs/

Municipal data from environmental pollution stations: https://analisi.transparenciacatalunya.cat/Medi-Ambient/Dades-d-immissi-dels-punts-de-mesurament-de-la-Xar/uy6k-2s8r/data

## Methods.
Linear regression model: Where the distribution of a single response variable (Y= standardized crude rate per 10,000 inhabitants) is related to several explanatory variables, X1, X2, . , by a regression model Monleon, 2017.<br>
Relative Risk: the RR (relative risk) or risk ratio as a tool calculated by the linear regression models [RR=1+(slope/intercept)] using ecological studies.The calculation of the relative ecological risk approximation as a method to approximate RR related to COVID-19 from the aggregated data is presented below, using the method proposed by Morgenstern.<br>
Statistics analysis: R Studio .<br>

## Variables of Ecological Study.
The aggregated data consists of 233 health areas in the rows (sanitary area) compiled in a spreadsheet by these different databases where the following variables are the columns:<br> 
●	health_area: part of the municipality where the incidence of COVID19 has been noted. It is related to a sanitary area where a certain number of inhabitants is controlled.<br>
●	municipality: Municipality or village of Catalonia.<br>
●	positive_cases: Total positive cases.<br>
●	suspected_cases: Total suspected cases.<br>
●	raw_rate_10k: raw rate per 10,000 inhabitants.<br>
●	standar_rate_10k: Standardized crude rate per 10,000 inhabitants.<br>
●	insured_people: Insured people in the area.<br>
●	surface_km2: Area occupied by the health area.<br>
●	density: Population density by km2.<br>
●	NOX_reduction_january2020: Reduction of the percentage of NOx in January 2020 compared to the previous 3 years.<br>
●	NOX_reduction_february2020: Reduction of the percentage of NOx in February 2020 compared to the previous 3 years.<br>
●	NOX_reduction_march2020: Reduction of the percentage of NOx in March 2020 compared to the previous 3 years.<br>
●	NOX_reduction_april2020: Reduction of the percentage of NOx in April 2020 compared to the previous 3 years.<br>
●	NOX_reduction_may2020: Decrease in the percentage of NOx in May 2020 compared to the previous 3 years.<br>
●	income_euros: Family income (thousands of euros). Catalan acronym called “RFBD”.<br>
●	income_euros_inhab: Family income per inhabitant (thousands of euros).<br>
●	income_index_100: Family income per inhabitant (index between 0-100%) referred to the whole of Catalonia.<br>

### Contact us:
Nicolas Ayala Aldana <br>
Department of Microbiology, Genetics and Statistics - University of Barcelona <br>
nayalaaldana@gmail.com ; nayalaal28@alumnes.ub.edu <br>

Dr. Antonio Monleon Getino <br>
Department of Microbiology, Genetics and Statistics - University of Barcelona <br>
amonleong@ub.edu <br>

Dr. Jaume Canela Soler <br>
Department of Preventive Medicine and Public Health - Hospital Clinic, University of Barcelona <br>
jcanela@ub.edu <br>



# disease_sim
# Scraped Webpages
https://en.wikipedia.org/wiki/List_of_international_airports_by_country
https://en.wikipedia.org/wiki/List_of_countries_and_territories_by_land_borders
https://en.wikipedia.org/wiki/List_of_countries_and_dependencies_by_population
# Introduction
Hello! Thank you for taking the time to look at my disease simulator!! Just some quick understanding. So First, I decided that the best way to build this model was by scraping data from Wikipedia. In the folders data parsing and CSV files, you can find the python notebooks that I used to pull data from Wikipedia, along with the CSV files that I derived from them. For simplicity's sake, I only chose to keep Airports that reported either a passenger role or an annual volume of passengers. 

Large (18,500,000+ Annual Passengers)
Medium (3,500,000–18,499,999 Annual Passengers)
Small (500,000–3,499,999 Annual Passengers)
Non-Hub (10,000–499,999 Annual Passengers)
Reliever (1–9,999 Annual Passengers)

Secondly, Annual Passengers are the reported volume of passengers.
The second CSV file is the population, which will be used for realistic modeling as much as possible.
Third, there is the bordering country CSV. This is a column of every border shared between every country in the world. Each border is listed only once.
## The math
https://en.wikipedia.org/wiki/Mathematical_modelling_of_infectious_disease
https://www.maa.org/press/periodicals/loci/joma/the-sir-model-for-spread-of-disease-the-differential-equation-model
I was unsure what model would be the best for modeling disease. Still, after some initial research, I believe that the best model to build a simulator would be to use the SIR model developed by W. O. Kermack and A. G. McKendrick. This has three categories
S(i)=Suseptible individuals
These are individuals that have not been infected with the disease
I(i)=Infected individuals
These individuals actively have the disease and can spread it to others.
R(i)=Recovered individuals
These are individuals who recovered from the disease
D(i)=Deceased individuals
These are individuals that died from the disease(Recovered and Deceased are placed into R(i) in the initial model, which is why the acronym is SIR)
## Transmission across Borders
## Transmission by Airports

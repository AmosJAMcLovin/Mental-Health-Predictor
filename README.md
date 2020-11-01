# Mental Health vs Suicide: Predicting Suicide Rates from Mental Health Risk Factors

<img src="Image/worldmentalhealthday_16x9.jpg" height="500" width="900" />


## Background

Mental health has become one of the greatest global health concerns according to the WHO (World Health Organization, 2017). It has critically high and increasing prevalence, yielding severe health outcomes. 

It is observed that 1 in 4 adults suffers from a diagnosable mental illness in any given year (National Alliance on Mental Health, 2013). According to WHO, there has been a 13% increase in mental health conditions overall from the last decade or so. Suicide rates on the other hand, have also [increased]( https://github.com/QianyueMa/Google-Health-Search-Project). WHO’s published statistics indicates that about 800,000 people die due to suicide every year, not to mention how many more people have attempted or idealized suicide. Especially among teenagers from ages 15-19, suicide is the third leading cause of death. 

So naturally their mental health concerns are important health risks that warrant further investigation. Considering the established strong correlation between suicide attempts or thoughts and underlying mental health conditions, our team believes it would be valuable **to study which personal and macroeconomic risk factors could predict the suicide rates on the national level and beyond**. 

- - -

## Project Objectives

### Main Question of Interest

* **To predict national suicide rates from the observed personal and macroeconomic mental health risk factors**
* (**this is a maybe*) To build an APP, in which people could enter their own data in the GDP/population/etc. input fields about their town/city/country to see if a policy change could predict lower suicide rates e.g.) The GDP increased in my town by 20% this year, so the policy-makers wonder if the government's investment on the health sector also increased, will the suicide rate decrease next year?

### Methodology & Objectives

We will conduct **statistical analysis about various risk factors**, **perform a set of data visualizations**, **build and test machine learning models**, in order to answer following **main questions**:

* Overall, what are the **strongest predictors for suicide* in different countries? Also, how to build **machine learning models* to study and predict our findings?
* On the **individual* level, how does the fact that a person had or has not sought for treatments influence their suicide risks? And why did they seek or not seek help for their mental health conditions? 
	* For example, the risk factors include the financial concerns (e.g., the insurance options offered, the company’s welfare packages), the fear of the consequences such as prejudice or employability if they disclose their mental health situations. It should be noted that those microeconomic factors are largely tied up to their country’s general macroeconomic factors as well. 
	* Those insights are generated from our [OSMI Mental Health in Tech Survey]( https://www.kaggle.com/ekwiecinska96/mental-health-in-techology-survey-2014-and-2016). 
* In terms of the **macroeconomic* factors, how does a country’s GDP/Income level average life expectancy, gender-specific fertility rate, education attainment, poverty rates and other socio-economic and demographic factors that affect the country’s yearly suicide rates? What causes the difference in suicide risks based on geographical location?
	* It is speculated that those mentioned national socio-economic factors determine the country’s holistic conservativeness level or attitude towards mental health topics. This attitude in turn will determine government’s funding ratio on the mental health sector, the severity of cultural stigma about mental illness, etc., which then play a large role in contributing to people’s decision about whether or not seeking treatment for their mental conditions and maybe also their risk of suicide. 
	* Those findings are observed from the World Bank’s [World Development Indicators](https://databank.worldbank.org/source/world-development-indicators) database. 


## Data Sources

Our project uses the insights generated from [Mental Health in Tech Survey from Open Sourcing Mental Illness (OSMI)]( https://www.kaggle.com/ekwiecinska96/mental-health-in-techology-survey-2014-and-2016) and the data from the [World Development Indicators database](https://databank.worldbank.org/source/world-development-indicators) from the World Bank. 

### Data Source 1
The survey data from the [OSMI mental health in technology surveys)]( https://www.kaggle.com/ekwiecinska96/mental-health-in-techology-survey-2014-and-2016)  are used to facilitate statistical analysis and to infer from its descriptive data representations.

The dataset contains 27 factors that could be segmented into **3 clusters of interests for our explanatory variables**. 

   - **Demographics**: age, gender, country, etc.
   - **Mental health services accessibility**: potential work interference, easiness to take a medical leave, insurance options, welfare benefits offered by employers, etc.
   - **Organizational cultures in the workplace in terms of openness about mental health**: easiness to discuss about mental health among co-workers, fear of negative consequences caused by disclosure, etc.

This is the detailed factor list **directly obtained* from this survey dataset's [notebook here](https://www.kaggle.com/osmi/mental-health-in-tech-survey/home):
 <img src="Image/data_map.png" height="500" width="900" />
 
### Data Source 2
We have obtained the macro-socio-economic factors extracted from the [World Bank’s World Development Indicators database](https://databank.worldbank.org/source/world-development-indicators). This dataset looks into 246 countries of low- or middle- or high-income levels across the continents. 

The **selected factors** include: 
- Gender-specific suicide mortality rate (per 100,000 population)
- Gender-specific life expectancy at birth, total (years)
- Population, total
- Gender-specific labour force participation rate, female (% of female population ages 15+) (national estimate)
- Gender-specific labour force with advanced education (% of total working-age population with advanced education)
- Gender-specific employment to population ratio, 15+, total (%) (national estimate)
- Educational attainment, at least completed primary, population 25+ years, total (%) (cumulative)
- Coverage of unemployment benefits and ALMP (% of population)
- Coverage of social safety net programs (% of population)
- Coverage of social insurance programs (% of population)
- Multidimensional poverty index (scale 0-1)


## So... The Columns/Factors included in the New Composite Dataset:

**(N.B. to be finalized...)*

countries, years, age, gender, sought_treatment(=1, =0), fear_negative_consequences, workplace_openness, financial_concerns; gdp, life-expectancy, population, labour_participation (by gender), employment_to_population_ratio (by gender), adequate_educational_attainment, unemployment_benefits_coverage, social_insurance_coverage, social_safety_net_coverage, poverty_index, **suicide_rates (by gender)**

The `suicide mortality rate` is the dependent variable. The rest of the factors are independent variables. The `countries` is one of the key features.

- - -

 ## Data Visualization and Analysis Processes
 
 - Data Cleaning 
     - Python Pandas 
 - Database 
     -  Postgresql
 - Exploratory analysis and visualization on the major variables
     - Python Matplotlib, Tableau, JavaScript Plotly, JavaScript D3.js, JavaScript Leaflet 
 - Front End 
     - HTML, CSS, Bootstrap, JavaScript
 - Machine Learning Models
     - Machine Learning Models: Linear Regression, Logistic Regression, Decision Tree, Random Forest, Support Vector Machine (SVM) Models and Natural Language Processing (NLP) algorithm
 - Deployment 
     - Heroku
 
## Architectural Diagram

<img src="Image/arctectured.png" height="500" width="900" />

- - -

  ## Tasks 
 
- Merging data sources, cleaning and processing the data
- Performing the exploratory analysis and creating data visualization - Amanda Qianyue Ma, Maria Loren
- Building an APP interface - Ermias Gaga
- Building ML, and NLP classification - Amos Johnson, Adedamola Atekoja (‘Damola)
  

 - - -

## References:
* World Health Organization. (2020). Mental Health. Retrieved October 31, 2020, from https://www.who.int/health-topics/mental-health#tab=tab_2
* World Health Organization. (2019). Suicide. Retrieved October 31, 2020, from https://www.who.int/news-room/fact-sheets/detail/suicide
* National Alliance on Mental Health. (2013). Mental Health Conditions. Retrieved October 31, 2020, from https://www.nami.org/Learn-More/Mental-Health-Conditions
* World Health Organization. (2017). Depression and other common mental disorders: global health estimates. Retrieved October 31, 2020, from https://www.who.int/mental_health/management/depression/prevalence_global_health_estimates/en/
* The World Bank, World Development Indicators (2020). Retrieved October 31, 2020, from https://databank.worldbank.org/source/world-development-indicators

### Algorithims were run again with scaled column and compared

### Additional plots, code explanations, ml evaluation plots, removal unecessary plots.

### 5th diagnosis added to data, Central tendency measures and std added to extract additional insights, normal distribution plots to compare pre and post covid data, line charts to support pie charts, updated figures in binom prob and visualisations, additional diagnosis added to ml model, confusion matrix plotted, removal of gender data for better continuinity of information flow

## Machine Learning models added- Part IV
### Decision Trees and Logistic Regression, hyper params and grid cv added, LogReg needs some extra tuning



## Data Prep for Machine Learning- Part III
### Encoded categorical variables, dropped column year, encoding returning true and false even after setting the dtype as category so replaced true false with boolean 1, 0,  checked the value counts of each target variable (Public and Private) Data was imbalanced- rebalanced with SMOTE

***

## Binomial distribution added on smaller sample- Part II

***

## Binomial distribution added on larger sample- Part II

***

# Changes made to data
## Datasets reduced to Two. 
## Clearer notebook layout
### The population chosen are adults who were inpatients in psychiatric facilities. 
## The data has been sourced from the CSO accesible at https://data.cso.ie/table/HR010 and https://data.cso.ie/table/HR014
## The objective, Identify early trends emerging in psychiatric inpatients based on hospital type, diagnosis and gender. Build classification model, to classify hospital type (Public or Private) based on inpatient diagnosis & classify to classify hospital type (Public or Private) based on inpatient gender.

*** 

# 🔶 Data Limitations
## Time range- pre 2019 data was in time steps of three as opposed to y.o.y as seen in 2019-2022 data.  disruptions to inpatient totals, for example, many hospitals experienced some level of closures due to outbreaks during COVID-19. Post covid data is continuing to be developed.

***

# The environment
## 📙 Jupyter Notebook 
### Chosen for neat workflow with markdown allowing for comprehensive sectioning
### Interactive with other libraries making it easy to clean, transform, visualise, model and evaluate all ends of the analysis.

*** 

# The language
## 🐍 Python - Has a variety of libraries for data science and easy to use syntax.

***

# The libraries
## 📚 Pandas, used for reading in the data and manipulation of the data. 
## 📚 Matplotlib.pyplot and Seaborn, easy to generate visualisations, great for quick plotting before finalising.
## 📚 Plotly, excellent for generating highly visual, interactive and appealing plots has a lot of extra functionality when used with dash to create more complex functions such as drop downs and animations. In this project Plotly is used to visualise the final version of a plot for communication of information. 
## 📚 Plotly.graph_objs module is great for creating more complex charts and in the context of this notebook, it was used for plotting multiclass graphs.

***

# 🚧CRISP-DM-
## Chosen as the method of project managment- easy to implement, 6 phases providing good control over workflow, encourages best practise through the 6 stages and has an iterative approach best seen in modelling.

***

# 💼 Business Understanding- Phase 1

As stipulated by B.Gavin, J.Lyne and F.Mc Nicholas, the lasting impact of COVID-19 on mental health, is as yet unkown. The anticipation surrounding the emerging data is expected to be highly impactful. (B.Gavin et al., 2020) Addressed in a paper by T. Frawley et al., 2020, emergency policymaking focused heavily on the "physical aspects and consequences of the viral infection", with little to no emphasis on the psychosocial impact. (T. Frawley et al., 2020,)

Interruption to social care arrangements, leisure services as well as reduced family incomes, due to COVID-19, were all reported to have had  negative impacts on the households quality of life according to a qualitative study which interviewed 40 families. (O’Sullivan et al., 2021, p. 1062) As part of the strategy to mitigate the risks associated with COVID-19, Ireland developed a 5 levels restrictions table which was based on the threat level of the virus. The top-level restrictions were enforced across the Republic of Ireland on three occasions, firstly on:

Wednesday, October 21, 2020, and were in place for a period of 6 weeks (O’Shea., K, 2020).

The second Level 5 restrictions started from midnight on Thursday, December 24, 2020, and were initially set to last until Tuesday, January 12, 2021.(Gov.ie. 2020)

The third updated Level 5 restrictions from midnight on Thursday, December 31, 2020, and remained in place until Sunday, January 31st 2021. (Gov.ie. 2020)

The impact of COVID-19 on mental health, was described in a persepctive piece, as being likely to have a larger psychosocial footprint than medical. The paper outlines subgroups of the population expected to experience increased mental health burdens as well as the anticipated corresponding diagnosis which include; Depressive disorders, anxiety, OCD and PTSD.(K.O'Connor et al, 2020) In agreeance, but from the perspective phhysical excercise, pre-pandemic studies such as Korczak et al., 2016 discussed the association of increased physical activity with lower prevalences of depressive symptoms. Knowing that the policies associated with COVID-19 decreased access to gyms, team sports, encouraged desk sitting and promoted isolation, it is the objective of this analysis to identify the prevalence/emergence of the diagnosis between the years 2019-2022. (For better understanding of the diagnosis please refer to the appendix section of this report for a detailed overview of the Approximate Synonyms and clinical information sourced from ICD-10data.com).

***


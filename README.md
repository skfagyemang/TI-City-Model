# TI-City-Model


### What is it?
The repository contains an urban expansion model developed to predict future residential development in an African city.
The model, which is named TI-City, combines agent-based and cellular automata modelling techniques to predict the geospatial behaviour of key urban development actors, including households, real estate developers and government.

To demonstrate the utility of the model, it has been applied to Accra city-region, Ghana, which is one of the largest city-regions in Africa. See Agyemang et al. (2022) for the underlying paper.

The model can be useful to African urban studies scholars, environmental and climate scientists, as well as city planners and urban policy makers in Africa.

The model is implemented in NetLogo programming platform.

The "TI-Model.zip" file contains the model and data for Accra. There are two versions of the model:
- "TI-City_validation", which contains parameterization used to validate the model; and
- "TI-City_prediction2030", which contains parameterization used to predict urban expansion of Accra up to 2030.


### How it works

TI-City has several key parameters. This includes:
 
1. A development control parameter, which accounts for diverse regulatory contexts;

2. Projected market demand for plots from households; 

3. Estimated share of households in low-, middle-, and high-income classes; 

4. Estimated demand for plots from real estate developers; 

5. Estimated share of real estate developers targeting middle and high income buyers; 

6. Land prices and affordability
 
7. Utility of land parcels; and 

8. The sensitivity of development to slope. 

The model computes the suitability and utility of a given parcel for each income group by considering the geographical characteristics of the parcel. In calculating utility, the model accounts for the parcel’s geographical characteristics weighted differently depending on the income group of prospective inhabitants. The utility is dynamically updated during the simulation based on the income characteristics in the geographic neighbourhood of each cell.
 

### How to use it

1. Select the simulation period. The unit is in years.

2. Select the number of households to simulate using the household slider.

3. Split households in low-, middle-, and high income classes using the sliders. The sum of the three proportions should be equal to 100 percent.

4. Select the number of real estate developers to simulate.

5. Split real estate developers into middle and high end suppliers. The sum of the two proportions should be equal to 100 percent.

6. Select slope coefficient, which determines the extent to which development patterns are influenced by slope. This is modelled after SLEUTH.

7. Select critical slope. This is the percent slope value beyond which development cannot occur. It may be derived from local urban development policies and regulations.

8. Select development control value. This determines the extent to which development conforms to government regulation/local plan. The lower the value the weaker the development control.


### Things to notice

The spatial resolution of the model as applied to Accra is 200m. This is about 50 times larger than the average size of land parcels in the city. To apply the model to Accra using the available data, the parcel enlargement factor should be considered in determining the number of households and real estate developers to simulate.

To adapt the model to any other city, consider the spatial resolution of the data and the extent to which is enlarges or reduces actual sizes of land parcels. Like the case of Accra, this could influence the number of households and real estate developers to simulate.


#### Key for income status predictions:
0 = undeveloped lands;
1 = Low income;
2 = Middle income;
3 = High income;
4 = seed year built-up.


#### Key for legal status predictions:
0 = undeveloped lands;
1 = informal development;
2 = formal development;
6 = seed year built-up. 


### Things to try

Consider adjusting some of the parameters. For instance, what happens with strong development control or what happens if there is a higher share of middle or high income households?

Experiment with data from a different city.


### Extending the model

Generalize TI-City as a global urban expansion model. There are ongoing plans to do this.

Integrate residential relocation and densification (vertical development) into the model.

Weight the influence of slope by the socio-economic characteristics of neighbourhoods and prospective inhabitants.


### Related model

SLEUTH


### How to cite it

Agyemang, F.S., Silva, E., & Fox, S. (2021). Modelling and simulating ‘informal urbanization’: An integrated ABM and CA model of urban residential growth in Ghana. Environment and Planning B: Urban Analytics and City Science. https://doi.org/10.1177%2F23998083211068843.


### References

Agyemang, F.S., Silva, E., & Fox, S. (2021). Modelling and simulating ‘informal urbanization’: An integrated ABM and CA model of urban residential growth in Ghana. Accepted for publication in Environment and Planning B: Urban Analytics and City Science.

Clarke, K. C., Hoppen, S., & Gaydos, L. (1997). A self-modifying cellular automaton model of historical urbanization in the San Francisco Bay area. Environment and Planning B: Planning and Design, 24(2), 247-261.

Zhou, Y. (2015). Urban growth model in Netlogo. Available at: http://www.gisagents.org/2015/09/urban-growth-model-in-netlogo.html

### Contact


Dr Felix S. K Agyemang; School of Geographical Sciences; Unversity of Bristol

Email: felix.agyemang@bristol.ac.uk

Profile: https://research-information.bris.ac.uk/en/persons/felix-s-k-agyemang

### LCI-estimation-of-wind-turbine

This work aims to generate the life cycle inventory (LCI) of wind turbines with machine learning algorithms and also some mathematical methods.

The data used in this work is from Danish Ministry of Energy (https://ens.dk/en) and some results from Dr. Romain Sacchi (https://github.com/romainsacchi/LCA_WIND_DK/blob/master/Complete_dataframe.csv).

Machine learning algorithms are able to estimate some parameters like Rotor Diameter and Tower Hub Height, and then get the mass of Rotor, Nacelle and Tower. Due to lack of data, the other parts of wind turbines like Foundation, Transformers and Power Cabbles are sized by some mathematical methods based on some reports and publications.

The prediction result of life time is not very satisfying, two labels were applied and they are the service time itself and decomission year of the wind turbine. However, the result is better than just setting 20 years as the life time for all the wind turbines.
It is possible to predict the total electricity production of wind turbines even without knowing the service time, and the result is acceptable compared with the way by using yearly average capacity factors.

The materials breakdown is achived by using interpolation or average values based on the detailed information of 5 wind turbines with different capacities. And the materials breakdown for foundations depend on the locations, monopile is assumed as the foundation type for offshore wind turbines as it is up to 80%.

Meanwhile, there are many assumptions for estimatiing the input materials, like the layout of the wind farm, activities involved in transport, assembly, end_of_life disposal and maintenance.

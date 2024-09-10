# module-11
Car price prediction

Data analysis by grouping data based on state

- As per bar plot - total_car_count_distrubution_per_state- Most car are sold in ca, followed by fl and ny
- As per bar plot- total_price_distribution_per_state- Total price of car sold are in ca, fl and ny order which is matching with total_car_count_distrubution_per_state observation. This mean there is a higher change of car being sold in ca, fl and ny states
- Even though car are easier to sell in ca, fl and ny, mean selling price in more in ak, tn and wy state as represented in total_mean_price_distribution_per_state bar graph

Data analysis by grouping data based on manufacture

- Bar plot= total_distribution_per_manufacture indicates most car sold are by Ford followed by Chevrolet and Toyota.

Car sale by grouping paint color

- Bar plot-distribution_per_color indicate car with white paint are sold most followed by black and silver color.


Above plots can help dealer to estimate which state consume most car, which state has the highest mean price for the car, which manufacture car are bought frequently and for which color.

Scatter plot indicate car sale have increased w.r.t to year time frame. This is expected as more car transactions happens now.

Modeling

There are multiple columns with non numeric data in the dataset.
To analyze non numeric features, I used Label encoder to assign unique numeric values for the feature.
I restricted the modeling to limited set of features to simplify modeling.

Linear regression
I fit a linear regression model on dataset with label encoder used for manufacture, fuel type, selling type and transmission. With the modeling MSE of the model is- 154685695.04151982

Ridge regression
I created a pipeline with Ridge regression and used gridsearchCV to try modeling with different values of the alpha.

Above MSE indicate ridge modelling performed slightly better than linear regression modelling as MSE of ridge model on data set is less than linear regression model

Above model can help dealer to predict the selling price of a new dataset.

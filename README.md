# Carbon-Capture-analysis
Carbon capture is a new emerging technology which can help to prevent the climate change and global sea level rising due to the increase in earth's temperature.
This repository contains the self project on finding the optimum Metallic Organic Framework Materials for Carbon capture using Machine Leaning techniques
I have given a quick desciption abput the analysis I have carried out in the markdown.
The dataset is available at the link : https://archive.materialscloud.org/record/2018.0016/v3

## Main Aspects

1. The MOFs dataset is taken from the data driven design of MOFs for wet flue gas CO2 Capture. It has more than 3,70,000 hypoythetical MOFs which are not yet synthesized but based on the properties we will sort these out.
2. First set is cleaning the dataset to remove all the NAN and the infinite values in the dataset. I have used pandas library to load the dataset and converted all the infinite values to the NAN and then remove these NAN values.
3. We see that there is discripency in the number of MOFs in some of the features ex. heat_adsorbtion at P0.15bar. This is because of the removal of infinite values.
4. A histogram is plotted to check which topology is mostly found in the dataset.

## Analysis tools used:

1. Descriptive analysis: For finding the right properties firstly correlation analysis is done to check how well the features are correlated to each other.
2. Distribution analysis: After finding the right properties I have checked the distribution, they follow w.r.t the CO2/N2 selectivity which is done by scatter and box plot.
3. Linear Regression: After sufficient information from the data, it is found that missing data may pose a biasness and inaccuracies in data. I have taken 150,000 datapoints for the regression analysis. The best 3 parameters are check for the multidimensional plotting and graphical representation of predicted vs actual values are shown.
4. Neural Network: Tensorflow library is used to create a dense neural network showing a low training loss of 0.14 which proves that these 3 features are sufficient to predict the best performing NNs.

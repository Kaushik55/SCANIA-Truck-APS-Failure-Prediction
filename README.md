# SCANIA-Truck-APS-Failure-Prediction
Air Pressure System (APS) in trucks generates pressurized air that is used for various functions of trucks such as braking and gear changes. Lot of money is spent on un-necessary checks done by service person on APS system in trucks, which can be prevented by developing a machine learning model that can predict the failure of component in APS. In this way, service can be restricted to the trucks whose APS component is predicted to be failed by the model.

Data is collected from UCI machine learning repository. The dataset consists of data from heavy Scania trucks in everyday usage. There are total 60000 data points in train data and 16000 data points in test data. The datasets positive class consists of component failures for a specific component of the APS system. The negative class consists of trucks with failures for components not related to the APS. 
There are total 171 features in the data set. The attribute names of the data have been anonymised for proprietary reasons. It consists of both single numerical counters and histograms consisting of bins with different conditions. There are 7 histogram features which are divided into 10 bins. 

Challenge Metric: 

Total Cost of prediction model = Cost1 * number of False Positives + Cost2 * number of False Negatives
Cost1 - Cost that an un-necessary check needs to be done by an mechanic (10$)
Cost2 - Cost of missing a faulty truck, which may cause a breakdown (500$)

Here, false positives (type 1 error) refer to model predicting failure in APS components even if there is no failure in reality. False Negatives (type2 error) refer to model predicting that there is no failure in APS component even there is failure in reality. Type2 error is very expensive and it may cause break down of truck, hence the cost associated with type2 error is more compared to type1


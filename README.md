# Beijing Housing Price Classification:
1. Two kinds of labels are generated based on unit price
	* 1.1 Equally spaced 
	* 1.2 Equally area   

The purpose of doing is to see how labels could influence the result. As we know, for labels are given by people’s will, for example, movie rating and etc. So i got the freedom to choose the way that i would like to label the data. While plotting all the data with many bins, new found it actually follows Gaussian distribution, in this way, the label generated should also follow gaussian distribution closely, which turns out it does! 


And the second method of labeling is just an extreme experiment, that i want to create a method of labeling that has the exact same number of samples for each class. After i plotted the price map based on equally area label, it turns out that it wasn’t a good way of labeling. 
Staring here, only equally spaced labeling method was applied to do the classification. Six models were applied:

   * 1. Gradient Boosting Classifier: 46.1%
   * 2. Random Forest Classifier:     43.8%
   * 3. Neural Network:               43.2%
   * 4. Decision Tree Classifier:     38.3%
   * 5. KNeighbors:                   36.6%
   * 6. SVM:                          29.2%
   
Consider that the dataset is time related. As we known from time series, timing has a huge influence in unit price as well. Base on this, think of some close edge situations, we give it a 1 class tolerance and would like to see how that works. Here goes the result:

   * 1. Neural Network:               87.3%
   * 2. Gradient Boosting Classifier: 87.0%
   * 3. Random Forest Classifier:     84.8%
   * 4. Decision Tree Classifier:     80.0%
   * 5. KNeighbors:                   74.3%
   * 6. SVM:                          68.2%

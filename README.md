# Identify customer segments with Arvato

In this project AZ Direct and Arvato Financial Solutions have provided two datasets one with demographic information about the people of Germany, and one with that same information for customers of a mail-order sales company. We applied unsupervised learning techniques on demographic and spending data for a sample of German households. We preprocess the data, apply dimensionality reduction techniques, and implement clustering algorithms to segment customers with the goal of optimizing customer outreach for a mail order company.

We look at relationships between demographics features, organize the population into clusters, and see how prevalent customers are in each of the segments obtained.

We are not allowed to publish the data provided by Arvato Financial Services due to the terms and conditions. In the notebook you can find the code and the analysis that I perfomed on the datasets.

# Installation
The following libraries are expected to be used in this project:

- NumPy
- pandas
- Sklearn / scikit-learn
- Matplotlib (for data visualization)
- Seaborn (for data visualization) The code should run with no issues using Python versions 3.*.

# Data
```Udacity_AZDIAS_Subset.csv```: Demographics data for the general population of Germany; 891211 persons (rows) x 85 features (columns).

```Udacity_CUSTOMERS_Subset.csv```: Demographics data for customers of a mail-order company; 191652 persons (rows) x 85 features (columns).

```Data_Dictionary.md```: Detailed information file about the features in the provided datasets.

```AZDIAS_Feature_Summary.csv```: Summary of feature attributes for demographics data; 85 features (rows) x 4 columns



Each row of the demographics files represents a single person, but also includes information outside of individuals, including information about their household, building, and neighborhood. We use this information to cluster the general population into groups with similar demographic properties. Then, we see how the people in the customers dataset fit into those created clusters. The hope here is that certain clusters are over-represented in the customers data, as compared to the general population; those over-represented clusters will be assumed to be part of the core userbase. This information can then be used for further applications, such as targeting for a marketing campaign.


# Results
- A good relatioship exists between the general and customers population data.
- The customers clusters are not universal i.e., the customers are not uniformly distributed in the general population with the population clusters so customers resides in certain clusters.
- The mail oreder company should target the clusters 2 and 16 where the customers data are over represented and neglect clusters 1,4, 10 where the customers clusters are under represented.
- The over-represented customer clusters shows that it belongs to category of older(45-60) and average income earners male.
On the other hand, the customers clusters that are underrepresented belong to the category of younger and average earners females. 


# Licensing, Authors, Acknowledgements
Credits must be given to Udacity for providing starting code for this project. The data was provided by Udacity partners at Bertelsmann Arvato Analytics.

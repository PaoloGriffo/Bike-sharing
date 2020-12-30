## A stability Index for an iterative procedure of selecting and validating a statistical model.

[MS Thesis in Statistical Sciences for decision - Federico II University of Naples project files.]
****************************************************************************************************************

The folder is structured as follow:

- [Bike sharing dataset](https://archive.ics.uci.edu/ml/datasets/bike+sharing+dataset) 
- Markdown Project code 'Bestfit_bikesharing.rmd' 
- Thesis Brochure 'MS_Thesis.pdf'

### Project scope and approach

The aim of the thesis is to develop an automatic statistical procedure able to select and validate a model introducing a Stability Index as decision-making rationale. 

A first application of general procedure is held for a Linear Regression case, facing the number of random accesses to a bike sharing service in Washington D.C. during the weekends in the years 2011 and 2012 as the varying weather conditions. 

A best model is selected with the Bestsubset selection (using BIC criteria) and a group of similar in best performing model is choosen using the Delta BIC criterion.

### Index derivation scheme

The Stability Index is computed on different partitions of the original data separately, considering both anomalous points and non, as follow: 

##### 1) Complete sample (2011-2012 records) 
##### 1.1) Complete sample (2011-2012 records) without anomalous (approx. 1%)
##### 2) First half of the sample (2011 records)  
##### 2.1) First half of the sample (2011 records) without anomalous (approx. 1%)
##### 3) Second half of the sample (2012 records)  
##### 3.1) Second half of the sample (2012 records) without anomalous (approx. 1%)

For these samples, the estimation, selection and validation steps of the best model are iterated B times, in turn resampling the B times with two different percentage, that is: 

##### a) 90% 
##### b) 80%

Finally, for the sake of clarity, a comparison between all the combinations stress the insights on the Stability Index.   




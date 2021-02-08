## A Stability Index for statistical models. An iterative procedure of selection and validation through the Delta BIC.

[MS Thesis in Statistical Sciences for decision - Federico II University of Naples project files.]
****************************************************************************************************************

This folder contains:

- [Bike sharing dataset](https://archive.ics.uci.edu/ml/datasets/bike+sharing+dataset) 
- Markdown Project code 'Bestfit_bikesharing.rmd' 
- Thesis Brochure 'MS_Thesis.pdf'

### Project scope and approach

The aim of the thesis is to develop a generalized and automatic procedure of selection and validation of a statistical model using the BIC criterion to derive a Stabiliy Index.

The Stability Index proposed in the thesis is tested in the case of the Linear Regression problem.  The UCI bike sharing dataset take into account the number of random accesses to the bike sharing service in Washington D.C. during the weekends in the years 2011 and 2012 and the varying weather conditions. 

A best model is selected with the Bestsubset selection (using BIC criteria) and a group of similar in best performing model is choosen using the Delta BIC criterion.

### Index derivation scheme

The Stability Index is computed on different partitions of the original data separately, considering both anomalous wheather conditions days and usuals ones, as follow: 

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




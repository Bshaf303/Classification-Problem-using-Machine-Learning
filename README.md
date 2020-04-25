Classification Problem using Machine Learning

This is a forest cover classification problem. The original data is located at: 
UCI Cover Type Dataset: https://archive.ics.uci.edu/ml/datasets/covertype
UCI dataset link: https://archive.ics.uci.edu/ml/machine-learning-databases/covtype/

The idea to do this project came from the Kaggle competition that ended September 24th, 2018 
and can be found here: https://www.kaggle.com/c/forest-cover-type-kernels-only

The dataset information can be found at:https://archive.ics.uci.edu/ml/datasets/covertype
In summary there are 581011 observations across 54 columns. The dependent variable is the "cover type" 
which are the trees found within the region. 

The data is derived from the remote sensing and GIS program at the department of forest services in conjuction 
with Colorado State University. The GIS panels come in 30 X 30 meter cells and each cell has attributes that 
are found in the data set. In addition to the GIS data there is also data from the US Geological Survey (USGS)
that is used to give attributes to the soil type found within the cells. The Soil Type is 40 binary columns alone. 

This project is done in RStudio starting with the exploratory analysis of the data and then we get into finding
the statistical significance of the variable relationships and finishing with various classification modeling
techniques to see if we can accurately predict the forest cover type on a test sample of the data. 

The data set is much too large to run in a local environment and maybe that's why it is up on Kaggle where users can 
utilize Kaggle's resources to compute. The other issue was the Kaggle data was pre-split into a training and test sets. 
the training set from Kaggle is 15,100 observations at 2.6% of the total data. This was not an ideal 70%/30% random split
ratio we have been taught in our data science program. The other issue is there was no distinct proportions for the
cover type dependent variable. Questioning the sampling method it was later decided to use the UCI data set and make 
appropriate random data splits in Rstudio. Issues quickly arose with local memory and processing resources being maxed out.
It was later decided to make an even smaller sample of data approximately 11,000 observations and then splitting that to
build and test the models. In theory a randomly sampled distribution of all variables is a valid method to build models on 
limited computing resources. In hindsight, renting a temporary server to run the data would be an option. 

The file that is attached is an RNotebook that was saved for teh github environment and simply uploaded to this platform. There are ways to interface R and Git, however, the proecessing time for this project has been too long even with a smaller sample of the data. It took 6 hours to run the notebook from the start mostly due to the training models used in many steps. There is a correct format in RStudio that can output RMarkdown into a .md file for Git. It was decided to forego this in regard to the processing time, saved for another day. 


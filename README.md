Getting-and-cleaning-data_assignment


This the repository for Coursera's Getting and Cleaning Data Assignment at week 4. It contains the 'codebook' which details the what data is collected, the source of the data, and a description of how the data is collected. It also lists a detailed description of the variables and measurements for the data aswell instructions on producing a tidy data set from these data files.

We first load the needed library.

Then we load all data, and we set up the names of the columns.

we then merge all data before extracting only data for mean or std information.

Using melt and dcast functions, we finally create the new tidy data set.

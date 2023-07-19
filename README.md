# TemperaturesDataImputation

## Introduction

This notebook aims to address the issue of data loss in temperature measurements taken at 10-minute intervals using Celsius as the unit of measurement. The dataset consists of 2007 records collected over 600-second periods. The objective is to perform data imputation using various mechanisms.

Temperature measurement is a fundamental concept in science and mathematics. It is a quantitative measure of the hotness or coldness of an object or environment. In this project, we will focus on temperature measured in Celsius, which is a widely used unit of temperature measurement.

The Celsius scale is based on the freezing point of water at 0 degrees Celsius and the boiling point of water at 100 degrees Celsius[4]. By understanding the principles of temperature measurement and the Celsius scale, we can effectively analyze and impute missing temperature data in our dataset.

To accomplish this, we will explore different techniques and algorithms for data imputation. Data imputation is the process of filling in missing values in a dataset using various statistical and computational methods. By applying these techniques to our temperature dataset, we can estimate and replace the missing temperature values, ensuring a more complete and accurate dataset for further analysis.

Throughout this notebook, we will leverage the power of Python programming language and its libraries to implement the data imputation techniques. Python provides a rich ecosystem of tools and libraries for data analysis and manipulation, making it an ideal choice for this project.

By the end of this notebook, we aim to have a comprehensive understanding of the data imputation process and have successfully imputed the missing temperature values in our dataset using various mechanisms. This will enable us to have a more complete and reliable dataset for further analysis and decision-making.

## Preprocessing

The first step in our data cleaning process is to remove erroneous values. To do so, we need to study how these values originate. One way to identify erroneous values is to use box plots. Box plots are a graphical representation of the distribution of a dataset, showing the median, quartiles, and outliers.

In our case, we can use a box plot to identify outliers in the temperature dataset. The outliers are characterized by very small values, which are unlikely to be accurate. Once we have identified the outliers, we can use a simple sequential algorithm to remove them[1].

Data imputation is another important step in preprocessing. Data imputation is the process of filling in missing values in a dataset using various statistical and computational methods. There are several techniques for data imputation, including mean imputation, median imputation, and mode imputation[3].

In our project, we will explore different techniques for data imputation and select the most appropriate one based on the characteristics of our dataset. We will use Python programming language and its libraries to implement the data imputation techniques[3].

Overall, preprocessing is a crucial step in data cleaning and analysis. It helps to ensure that the data is accurate, complete, and reliable, which is essential for making informed decisions based on the data. In the next section, we will explore different techniques for data imputation in more detail.

## Conclusion

In this project, we explored different techniques for data imputation to address the issue of data loss in temperature measurements taken at 10-minute intervals using Celsius as the unit of measurement. We used mean imputation, median imputation, LOCF, linear interpolation, and spline interpolation to fill in the missing values in the dataset.

After applying these techniques, we found that LOCF was the most effective method for imputing missing values in our dataset. With the dataset now complete, we used the LOCF method to detect the circadian temperature pattern.

Overall, data imputation is a crucial step in data cleaning and analysis. It helps to ensure that the data is accurate, complete, and reliable, which is essential for making informed decisions based on the data. By exploring different techniques for data imputation, we can select the most appropriate one based on the characteristics of our dataset and the research question.

In conclusion, this project highlights the importance of data cleaning and analysis in temperature measurement. With the right tools and techniques, we can effectively analyze and impute missing temperature data, ensuring a more complete and accurate dataset for further analysis and decision-making.

#### Types of Missing Values

- Missing Completely at Random (MCAR)
- Missing at Random (MAR)
- Missing Not at Random (MNAR)

#### Methods for Data Imputation

- Mean Imputation
- Median Imputation
- LOCF
- Linear Interpolation
- Spline Interpolation

Citations:
[1] https://towardsdatascience.com/data-cleaning-in-r-made-simple-1b77303b0b17
[2] http://pzs.dstu.dp.ua/DataMining/preprocessing/bibl/fimd.pdf
[3] https://vitalflux.com/pandas-impute-missing-values-mean-median-mode/
[4] https://stefvanbuuren.name/fimd/sec-monotone.html
[5] https://bookdown.org/aschmi11/RESMHandbook/data-preparation-and-cleaning-in-r.html
[6] https://epirhandbook.com/en/missing-data.html
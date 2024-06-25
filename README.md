# psywiz: Psychometric Wizardry Tools

## Overview

psywiz is an R package designed to simplify and enhance psychometric analysis workflows. It provides a collection of user-friendly functions for conducting common psychometric analyses, with a focus on Confirmatory Factor Analysis (CFA). The package is primarily built upon extracting and reordering results from lavaan (https://lavaan.ugent.be/).



## Installation

You can install the development version of psywiz from GitHub with:



```r
# install.packages("devtools") 
devtools::install_github("heelgueta/psywiz") 
```



## Main Features

### cfawiz: Confirmatory Factor Analysis Wizard



cfawiz is the primary function in psywiz, offering a streamlined approach to conducting CFA:



- Easily specify single or multiple factors and their indicators

- Support for correlated factor models

- Flexible estimator options, including multiple estimators in a single run

- Customizable output with color-coded factor loadings and fit indices

- Integration with variable descriptions for enhanced result interpretation

- Flexible fit indices reporting (short, long, full)

- Options for displaying both standardized and unstandardized loadings



## Usage



Here are some examples of how to use cfawiz:
(Asuming a df with vars such as ... scaleA1, scaleA2, scaleA3, scaleA4 that load on factor scaleA... and so on)

```r

r 
library(psywiz) 

# Single factor CFA with default estimator (DWLS) 
cfawiz(df, "scaleA") 

# Single factor CFA with multiple estimators 
cfawiz(df, "scale", estimator = "MULTI") 

# Two correlated factors CFA 
cfawiz(df, "scaleA,scaleB") 

# Three correlated factors CFA with multiple estimators and both loadings types 
cfawiz(df, "scaleA,scaleB,scaleC", estimator = "MULTI", loadings = "both") 

# CFA with full fit indices 
cfawiz(df, "scaleA,scaleB", fitindices = "full") 
```




## Features



- Flexible model specification for single and multiple factor models

- Support for various estimators, including ML, ULS, WLS, DWLS, MLR, ULSM, and ULSMV

- Color-coded output for easy interpretation of results

- Customizable fit indices reporting

- Options for standardized and unstandardized loadings

- Integration with variable descriptions

- Handling of ordered categorical variables



## Future Developments



- Enhanced visualization of CFA results

- Integration with other psychometric techniques (e.g., descriptives, IRT, EFA)

- Automated reporting functionalities

- Improved handling of missing data and non-normal distributions



## Contact



Herman Elgueta - herman.elgueta@umag.cl - Universidad de Magallanes



Project Link: https://github.com/heelgueta/psywiz


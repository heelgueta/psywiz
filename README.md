# psywiz: Psychometric Wizardry Tools 

## Overview 

psywiz is an R package designed to simplify and enhance psychometric analysis workflows. It provides a collection of user-friendly functions for conducting common psychometric analyses, with a focus on Confirmatory Factor Analysis (CFA). So far its mostly entirely based upon extracting and reordering results from lavaan (https://lavaan.ugent.be/).

## Installation 

You can install the development version of psywiz from GitHub with: 

```r
# install.packages("devtools")
devtools::install_github("yourusername/psywiz")
```

## Main Features 

### cfawiz: Confirmatory Factor Analysis Wizard 

`cfawiz` is the primary function in psywiz so far, offering a streamlined approach to conducting CFA: 

- Easily specify multiple factors and their indicators 
- Automatic handling of problematic items (not quite yet)
- Customizable output with color-coded factor loadings 
- Integration with variable descriptions for enhanced result interpretation 
- Flexible fit indices reporting 

## Usage 

Here's a basic example of how to use `cfawiz`: 

```r
library(psywiz)

# Assuming 'mydata' is your dataset, for a one factor CFA on items named "prefix01", "prefix02", "prefix03", "prefix04":
cfawiz(mydata, "prefix")
```

## Features in Development 

- Enhanced visualization of CFA results 
- Integration with other psychometric techniques (e.g., IRT, EFA) 
- Automated reporting functionalities 

## Contact 

Herman Elgueta - [herman.elgueta@umag.cl](mailto:herman.elgueta@umag.cl)

Project Link: [https://github.com/heelgueta/psywiz](https://github.com/heelgueta/psywiz)

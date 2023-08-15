Directory Structure
--------------------

    .
    ├── config  <- any configuration files, parameters and output results
    ├── data
    │   ├── 01_raw <- original unmodified data acting as source of truth and provenance
    │   ├── 02_interim <- data in intermediate processing stage
    │   ├── 03_processed <- data after all preprocessing has been done
    │   ├── 04_models <- compiled model .pkl or HDFS or .pb format
    │   ├── 05_model_output <- output model
    │   ├── 06_reporting <- data for reporting   
    │   └── 07_predictions <- predictions output data
    ├── notebooks <- jupyter notebooks for exploratory analysis and explanation "date-cs-title.ipynb"
    ├── references  <- usage documentation or reference papers
    ├── results <- generated project artefacts eg. visualisations or tables
    └── src - scripts for processing data eg. transformations, dataset merges etc.
    │   ├── d01_raw <- original unmodified data acting as source of truth and provenance
    │   ├── d02_interim <- data in intermediate processing stage
    │   ├── d03_processed <- data after all preprocessing has been done
    │   ├── d04_models <- scripts for generating models
    │   ├── d05_model_output <- output model
    │   ├── d06_reporting <- data for reporting
    │   ├── d07_visualization <- scripts for visualisation during EDA, modelling, error analysis etc. 
    │   ├── d08_predictions <- predictions output data 
    │   └── tools <- general tools
    ├── LICENSE
    ├── README.md
    |--- requirements.txt <- file with libraries and library versions for recreating the analysis environment
   
   ---
   # Assorment Creation
## Overview

This project is a solution to the business problem of reducing excess products or creating new products from existing ones. It uses a sample data source that resembles a dataset in the business. The techniques used require knowledge of matrix algebra and general data cleaning practices.

## Algorithm

The algorithm used to maximize the number of assortments/kits/bundles/sets that can be generated is to find the minimum amount or lower bound that restricts other combinations. It also displays a way to find the amount of continuous difference bundles that can be generated with a small variation. This answers the concern of generating off or orphan bundles in different sides of the spectrum.

## Usage

To use the project, you will need to have a sample data file in the same directory as the project code. The sample data file should be xlsx file with the following columns:

    characteristics: product or item features
    quantity: The quantity of the product

## Result 
This will generate a report that shows the number of assortments/kits/bundles/sets that can be generated, as well as the minimum amount or lower bound that restricts other combinations.

Contributing

If you would like to contribute to the project, please fork the repository and submit a pull request.

License

The project is licensed under the MIT License.

I hope this is helpful!
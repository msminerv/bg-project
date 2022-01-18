# Burning Glass Project

This repo contains all of the work for the burning glass research project at INSEAD. The following table of contents will guide you to the different sections of this project, which are mainly subdivided into data gathering, cleaning, and analysis.

Explanations and examples on how to run the code can be found within each section.

## Table of Contents

1. Objective
2. [Data](https://ramonprz01.github.io/bg-insead-project/data)
3. [Analysis](https://ramonprz01.github.io/bg-insead-project/analysis)


## 1. Objectives

> Infer organizational structure (vertical and horizontal) from job descriptions

What are we really after? It seems our goal is to measure two things:
How many layers of reporting are there in a given firm? [VERTICAL]
How many divisions are there in a given firm? [HORIZONTAL]

Or, can we capture variance across companies in terms of:
- Hierarchical layers
- Breadth of divisions

There are many ways to try to get at these constructs, but none are perfect.

## 2. [Data](https://ramonprz01.github.io/bg-insead-project/data)

The dataset was purchased from Burning Glass Technologies and it is a compilation of large number of job ads that have been posted by many companies over the last 13 years (2007-2020) and 2007.

The data comes with 57 variables and the dictionary is available in the data folder above.

### Size
- ~1TB for the full uncompressed data. (CSV files)
- ~650GB for the cleaned datasets. More details on the cleaning are available in the cleaning folder above. (CSV files)
- ~150GB for the cleaned datasets composed of only the observations with salary info in them. (parquet files)
- ~55GB for the cleaned 76k companies datasets. (parquet files)

Click on the link above to find more information about the variables.

## [Cleaning](https://ramonprz01.github.io/bg-insead-project/cleaning)

For the whole process on how to collect, extract, and clean the dataset, please visit the cleaning folder. For the cleaned datasets, please use the links below.

- [Cleaned Data](https://www.dropbox.com/sh/nmfhn03u5868e7f/AAAAhf4xB9lc_qbido0A1S-Ma?dl=0)
- [Cleaned 76k Companies Sample](https://www.dropbox.com/sh/4jleqjmw5rf7vd9/AADL_TwWFY93TCUPm6L87akua?dl=0)
- [Cleaned Salary Data](https://www.dropbox.com/sh/bxaenjocw9drj3o/AAChXPpMNteu2FHbQuNk-duHa?dl=0)

## 4. [Analysis](https://ramonprz01.github.io/bg-insead-project/analysis)

### Here is where to find what?

1. Clusters based on k-means 
    - Inside `analysis/approach_8` and also in `analysis/approach_1` folder
    - Notebooks 09 and 09p2
    - [Results-Data](https://www.dropbox.com/sh/24pgu3mtsdl7yv1/AACqPm0g5ACl7XwQOyEWueL2a?dl=0)
2. Occurrence of up-/downward-directed terms in ads
    - Inside `analysis/approach_8` folder
    - Notebook 07
    - [Results-Data](https://www.dropbox.com/sh/1k5k97hk7zgfzcu/AAAlx9RvcYco8decHzI7c_aBa?dl=0)
3. Occurrences of ‘reports to’ in ads
    - Inside `analysis/approach_8` folder
    - Notebook 07
    - [Results-Data](https://www.dropbox.com/sh/1k5k97hk7zgfzcu/AAAlx9RvcYco8decHzI7c_aBa?dl=0)
4. Number of salary brackets / peaks in the distribution
    - Not available as of 27-Nov-2020
    - [Results-Data with all salary observations available](https://www.dropbox.com/sh/bxaenjocw9drj3o/AAChXPpMNteu2FHbQuNk-duHa?dl=0)
5. Managerial intensity in job ads at the firm-year level
    - Inside `analysis/approach_8` folder
    - Notebook 08
    - [Results-Data](https://www.dropbox.com/sh/j4s031wc5vp89jd/AADdyOV_tKNKz_w309ySDRfka?dl=0)
6. Number of unique job posts, occupations and job titles per firm-week
    - Inside `analysis/approach_8` folder
    - Notebook 08
    - [Results-Data](https://www.dropbox.com/sh/j4s031wc5vp89jd/AADdyOV_tKNKz_w309ySDRfka?dl=0)
7. Any descriptives that you’ve produced at the industry level (e.g. 2- and 4-digit NAICS codes)

They are descriptives throughout a lot of the notebooks. There is no explicit notebook devoted to descriptives though. The details on the tasks below can be found in the output of the notebooks above.

    - How many companies hire in each code each year
    - How many unique job posts there are
    - Any details on missing data for these
        - This was done on the already cleaned data
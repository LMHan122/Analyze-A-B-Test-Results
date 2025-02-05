# Analyze A/B Test Results 

## Introduction

In this project, I will analyze the results of an A/B test conducted by an e-commerce company using three approaches:

1. Perform hypothesis testing by manually coding the statistical calculations.
2. Use built-in methods from the `statsmodels` library to conduct the same test.
3. Apply a logistic regression model to evaluate the impact of the new page on conversions.

The company has developed a new web page aimed at increasing the number of users who "convert"—i.e., those who choose to pay for the company's product. The objective is to assess whether the new page is more effective than the existing one. Specifically, I aim to determine whether the company should:

- Implement the new page,
- Retain the old page, or
- Continue the experiment to collect more data.

## Data

There are two CSV files provided as part of this project:

### `ab_data.csv`
This file contains 5 columns:

| Data Column     | Purpose                                                                 | Valid Values              |
|-----------------|-------------------------------------------------------------------------|---------------------------|
| `user_id`       | Unique identifier for each user                                         | Integer values            |
| `timestamp`     | The time when the user visited the webpage                               | Date and time             |
| `group`         | The user's assignment in the A/B experiment: `control` or `treatment`   | `['control', 'treatment']`|
| `landing_page`  | Whether the user visited the old page or the new page                    | `['old_page', 'new_page']`|
| `converted`     | Whether the user decided to pay for the product (1 for 'yes', 0 for 'no')| `[0, 1]`                  |

### `countries.csv`
This file contains 2 columns:

| Data Column | Purpose                                              | Valid Values   |
|-------------|------------------------------------------------------|----------------|
| `user_id`   | Unique identifier for each user                      | Integer values |
| `country`   | The country from which the user visited the website  | Country names  |

## File Overview

- `Analyze_ab_test_results_notebook.ipynb`: The Jupyter Notebook containing the A/B test analysis.
- `ab_data.csv`: The dataset used for analysis.
- `countries.csv`: The additional dataset containing user country information.
- `pyproject.toml`: Project configuration file.

## Project Setup

To set up the project, use the provided `pyproject.toml` for dependency management and environment configuration.

## Author & Contact

**Leslie Hanson**  
Email: [lesliemhanson@gmail.com](mailto:lesliemhanson@gmail.com)

## License

This project is licensed under the MIT License.


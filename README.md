# bootstrapping
bootstrapping application


# Call Center Efficiency Analysis

## Project Overview
This project aims to evaluate and compare the efficiency of two operational models, Apollo 1 and Apollo 2, used in a call center. The main metric of interest is the average call time under each model. We employ a statistical technique known as bootstrapping to estimate the variability and reliability of average call times for each model.

## Objective
To determine which call center model, Apollo 1 or Apollo 2, is more efficient in terms of managing call times. Efficiency is assessed by the mean call time and the variability of call times observed through bootstrapping simulations.

## Data Description
The dataset simulates call times over a period of one month, with alternating days under Apollo 1 and Apollo 2 models:
- `call_dt`: The date of calls.
- `model`: Indicates whether the call was handled under Apollo 1 or Apollo 2 model.
- `call_time`: The duration of each call in seconds.

## Methodology
Bootstrapping is used to generate distributions of mean call times for each model by resampling the data:
1. **Data Preparation**: Generate simulated data for call times under each model.
2. **Bootstrapping**: Perform repeated sampling with replacement from the dataset to compute the distribution of the mean call time for both models.
3. **Analysis**: Compare the distributions to assess which model consistently leads to lower average call times and less variability.

## Tools Used
- Python: Main programming language.
- Pandas: Data manipulation and analysis.
- NumPy: Numerical operations.
- Matplotlib and Seaborn: Data visualization to plot the results of the bootstrapping.

## Results
The analysis includes histograms and KDE plots that show the distribution of bootstrapped average call times for each model. Insights can be drawn from the comparison of these distributions regarding which model performs better in terms of efficiency and consistency.

## How to Run the Project
Ensure you have Python installed along with Pandas, NumPy, Matplotlib, and Seaborn. You can run the script `call_time_analysis.py`, which includes all the data simulation, bootstrapping logic, and plotting commands.

## Conclusion
This project provides a statistical framework to compare the efficiencies of different operational models in a call center, using bootstrapping to account for variability in the data and to make robust inferences about model performance.

## License
This project is licensed under the MIT License - see the LICENSE.md file for details.

## Authors
- Ender Sari endersari.com

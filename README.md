## COVID-19 SIR Model for Laval

This project uses the SIR (Susceptible-Infectious-Recovered) model to analyze the spread of COVID-19 in Laval, Canada. Due to discrepancies in reported data after January 2, 2022, this model approximates the missing cases using the infection rate from the previous 63 days.

## Data and Approach

- **Population**: Laval’s population (~400,000).
- **Time Frame**: October 31, 2021 - January 2, 2022.
- **Infection Rate (b)**: Estimated between 1.5/14 and 3.5/14 based on available research.
- **Recovery Rate (k)**: Assumed as 1/14 based on Quebec government guidelines.
- **Death Rate**: 1.7% based on data from Johns Hopkins University.

We used Euler’s method to approximate the solution of the SIR model and compare it with real data. Pearson’s coefficient was used to find the infection rate that best fits the real data.

## Key Findings

The model shows a significant underreporting of cases post-January 2, 2022. Our predicted model suggests up to 138,000 cases compared to the reported 62,000.

## Limitations

- **SIR Model Assumptions**: The model assumes a single epidemic wave, constant population, and uniform infection rates.
- **Simplifications**: Immunity and varying death rates were not factored in, which could affect long-term accuracy.

## Future Improvements

- Implement class-based system to optimize model readability.
- Include immunity and more granular death rate modeling.

## How to Use

To run the project, simply open the notebook in Google Colab:

1. Clone the repository or download the notebook.
2. Open [Google Colab](https://colab.research.google.com/).
3. Upload the notebook `SIR_Laval_Project.ipynb` to Colab.
4. Run the cells to simulate the SIR model and compare the results with real-world data.

# Random Walk Process

A **random walk** is a process in which there is an equal chance of moving up or down by a random number. A random walk is a series whose first difference is stationary and uncorrelated.

![Random Walk Process](ts1.png)

## Stationary vs Non-Stationary
A **stationary** time series is one whose statistical properties do not change over time. It has:
- Constant mean
- Constant variance
- Constant autocorrelation (independent of time)

### Differencing
**Differencing** is a transformation that calculates the change from one timestep to another:

\[ y'(t) = y(t) - y(t-1) \]

- **First-order differencing:** Taking the difference once.
- **Second-order differencing:** Taking the difference twice.

![Stationary vs Non-Stationary](ts2.png)

### 2.1 Mean Graph of Stationary vs Non-Stationary
![Mean Graph](ts3.png)

### 2.2 Variance of Stationary vs Non-Stationary
![Variance Graph](ts4.png)

## The Autocorrelation Function
- **Correlation** measures the extent of a linear relationship between two variables.
- **Autocorrelation** measures the linear relationship between lagged values of a time series.
- **Lag** refers to the number of timesteps separating two values.
- **ACF plot**: 
  - In a trending series, ACF coefficients decrease linearly with increasing lag.
  - In a seasonal series, ACF shows periodic patterns.

![Autocorrelation Function](ts5.png)

## Differenced Random Walk
![Differenced Random Walk](ts6.png)

## Autocorrelation for Above
![Autocorrelation for Differenced Random Walk](ts7.png)

## Google Stock Price Dataset
![Google Stock Price Dataset](ts8.png)

## Autocorrelation of the First Difference of Dataset
![Autocorrelation of First Difference](ts9.png)

## Train and Test Set
![Train and Test Set](ts10.png)

## Prediction Using Mean, Last Value, and Drift Method
![Prediction Methods](ts14.png)

## MSE Squared Loss of Above Methods
![MSE Squared Loss](ts15.png)


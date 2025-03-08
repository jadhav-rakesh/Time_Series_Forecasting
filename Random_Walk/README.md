# Random Walk Process

A **random walk** is a process in which there is an equal chance of moving up or down by a random number. It is a time series where the first difference is stationary and uncorrelated.

## Formula
The mathematical representation of a random walk is:

\[ y(t) = C + y(t-1) + \epsilon(t) \]

Where:
- **y(t)** is the value at the present time *t*.
- **C** is a constant.
- **y(t–1)** is the value at the previous timestep *t–1*.
- **ϵ(t)** is a random number (white noise) from a standard normal distribution with mean 0 and variance 1.

## Stationarity
A **stationary** time series has statistical properties that do not change over time. It has:
- Constant mean
- Constant variance
- Constant autocorrelation (independent of time)

### Transformation
A mathematical operation can be applied to a time series to make it stationary.

### Differencing
**Differencing** is a transformation that calculates the change between consecutive timesteps.

\[ y'(t) = y(t) - y(t-1) \]

- **First-order differencing:** Taking the difference once.
- **Second-order differencing:** Taking the difference twice.
- **Inverse transform:** Undoing a transformation to revert to the original scale.

## Testing for Stationarity
The **Augmented Dickey-Fuller (ADF) test** helps determine if a time series is stationary by testing for a unit root. If a unit root is present, the series is **not** stationary.

## The Autocorrelation Function (ACF)
- **Correlation** measures the linear relationship between two variables.
- **Autocorrelation** measures the linear relationship between lagged values of a time series.
- **Lag** is the number of timesteps separating two values.
- **ACF plot**: 
  - In a trending series, coefficients decrease linearly as lag increases.
  - In a seasonal series, ACF shows cyclical patterns.

## The Drift Method
The **drift method** for forecasting uses:

\[ \text{forecast} = \text{drift} \times \text{timestep} \]

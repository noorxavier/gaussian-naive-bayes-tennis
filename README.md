# Gaussian Naive Bayes — Tennis Prediction

A from-scratch implementation of **Gaussian Naive Bayes** for predicting whether tennis should be played based on numerical weather conditions.

The model uses:

- Temperature
- Humidity
- Wind Speed

to predict:

- `Yes` — Tennis should be played
- `No` — Tennis should not be played

---

## 📌 Problem Statement

Given a dataset containing 50 observations of weather conditions, predict whether tennis should be played for a new test case using the **Naive Bayes classification algorithm**.

Since all input features are numerical, the **Gaussian probability distribution** is used to calculate the likelihood of each feature given a class.

The Naive Bayes score is calculated as:

\[
Score(C) = P(C) \times P(T|C) \times P(H|C) \times P(W|C)
\]

where:

- \(C\) = class (`Yes` or `No`)
- \(T\) = Temperature
- \(H\) = Humidity
- \(W\) = Wind Speed

The class with the higher score is selected as the prediction.

---

## 📊 Dataset

The dataset contains **50 samples**.

### Features

| Feature | Description | Type |
|---|---|---|
| `Temperature_C` | Temperature in Celsius | Numerical |
| `Humidity_pct` | Humidity percentage | Numerical |
| `Wind_kmh` | Wind speed in km/h | Numerical |
| `Play` | Whether tennis should be played | Categorical |

### Target Classes

- `Yes`
- `No`

Dataset file:

```text
tennis_numerical_50_samples.csv

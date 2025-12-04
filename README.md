# AI Detect Straight Back

## Brief Description

This project utilizes Artificial Intelligence to detect and classify back posture. By analyzing distance measurements from a sensor, the system determines whether a person's back is straight or not. It compares a standard calibrated distance with the real-time measured distance to assess posture.

## Technique Used

The core technique used in this project is **K-Means Clustering**, an unsupervised machine learning algorithm.

- The model calculates the absolute difference between the `standard distance` and the `real distance`.
- It then clusters these differences into two categories (e.g., Straight Back vs. Not Straight Back).
- The model is implemented using Python and the `scikit-learn` library.

## Example Training Data

The model is trained on sensor data logged in `sensor_log.csv`. The dataset includes the following features:

- `standard distance`: The reference distance for a straight back.
- `real distance`: The actual distance measured by the sensor.

**Sample Data:**
| standard distance | real distance |
|-------------------|---------------|
| 44.0 | 44.0 |
| 44.0 | 46.0 |
| 44.0 | 47.0 |
| 44.0 | 34.0 |
| 44.0 | 59.0 |

## How to Clone the Project

To set up this project on your local machine, run the following command in your terminal:

```bash
git clone <repository-url>
cd ai-detect-straigh-back
```

### Prerequisites

- Python 3.x
- Jupyter Notebook
- Libraries: `pandas`, `matplotlib`, `scikit-learn`

You can install the required libraries using:

```bash
pip install pandas matplotlib scikit-learn
```

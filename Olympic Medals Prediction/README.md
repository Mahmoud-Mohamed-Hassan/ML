# Olympic Medal Prediction

This project uses a linear regression model to predict the number of Olympic medals a country will win based on historical data.

## Data

The data used in this project is from a CSV file named `teams.csv`.  It contains information about different countries' Olympic performances, including:

* **team:** The name of the country's team.
* **country:** The name of the country.
* **year:** The year of the Olympic games.
* **athletes:** The number of athletes representing the country.
* **age:** The average age of the athletes.
* **prev_medals:** The number of medals won by the country in the previous Olympics.
* **medals:** The number of medals won by the country in the current Olympics.

## Methodology


1. **Data Cleaning:**
   - Handled missing values by removing rows with any missing data.
   - Split the data into training and testing sets based on the year (before 2012 for training, 2012 and after for testing).


2. **Feature Selection:**
    - The model uses "athletes" and "prev_medals" as predictor variables.

3. **Model Training:**
   - Trained a linear regression model on the training data.

4. **Prediction:**
    - Applied the trained model to predict the number of medals for the test data.

5. **Error Evaluation:**
   - Calculated the Mean Absolute Error (MAE) to evaluate the model's performance on the test set.
   - Analyzed the errors by team and calculated the ratio of the average error to the average number of medals for each team.
   - Visualized the distribution of error ratios.


## Results

The linear regression model achieves a certain MAE value on the test set, indicating the average absolute difference between predicted and actual medal counts.  The analysis of error ratios by team provides insights into the model's performance for different countries, highlighting areas where the model may be less accurate.

## Future Improvements

* Try different machine learning models to see if they perform better than linear regression.
* Implement more sophisticated techniques for handling missing data.

## Usage

1. Make sure you have the required libraries installed (pandas, numpy, seaborn, matplotlib, scikit-learn).  You can use pip to install them (e.g., `pip install pandas numpy seaborn matplotlib scikit-learn`).
2. Place the `teams.csv` file in the same directory as the Python script.
3. Run the script to execute the analysis.

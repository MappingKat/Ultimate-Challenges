# Ultimate Data Analysis Project

This project involves three main parts:

1. Analyzing login data to understand user patterns.
2. Designing an experiment to encourage driver partners to serve two cities.
3. Building a predictive model to determine rider retention.

## Part I: Login Data Analysis

### Objective

Analyze login data to identify hourly, daily, weekly, and monthly patterns in user activity.

### Data Cleaning and Exploration

1. **Load and Inspect Data**:
   - Convert timestamps to datetime objects.
   - Check for missing and duplicate data.

2. **Resample Data**:
   - Aggregate login counts into 15-minute, hourly, daily, weekly, and monthly intervals.

3. **Handling Missing Values**:
   - Fill missing numeric values with the mean.
   - Use `SimpleImputer` for categorical columns.

### Patterns and Insights

1. **Hourly Patterns**:
   - Higher and more consistent login activity during weekdays.
   - Higher peaks during weekends.

2. **Daily Patterns**:
   - Regular daily activity with varying peaks indicating higher user engagement on specific days.

3. **Weekly Patterns**:
   - Increasing login activity over weeks.

4. **Monthly Patterns**:
   - Significant monthly variations indicating seasonal effects.

## Part II: Experiment and Metrics Design

### Objective

Design an experiment to encourage driver partners to serve both Gotham and Metropolis by reimbursing toll costs.

### Key Measure of Success

Increase in the number of driver partners serving both cities.

### Experiment Design

1. **Population Segmentation**:
   - Divide drivers into Control and Experimental groups.

2. **Reimbursement Scheme**:
   - Implement toll reimbursement for the Experimental group only.

3. **Duration**:
   - Run the experiment for 3 months.

4. **Data Collection**:
   - Track the number of trips involving crossing the toll bridge.

5. **Statistical Tests**:
   - Difference in Proportions Test.
   - Paired t-test (if applicable).

6. **Interpretation and Recommendations**:
   - Positive results: Implement policy permanently.
   - Negative results: Explore alternative incentives.

## Part III: Rider Retention Prediction

### Objective

Build a predictive model to determine whether a user will be active in their 6th month on the system.

### Data Cleaning and Exploration

1. **Load and Inspect Data**:
   - Convert date columns to datetime.
   - Create a 'retained' column to indicate user activity in the last 30 days.

2. **Handle Missing Values**:
   - Fill missing numeric values with the mean.
   - Use `SimpleImputer` for categorical columns.

3. **Exploratory Analysis**:
   - Visualize distribution of retained users.
   - Analyze trips in the first 30 days and average distance per trip by retention.
   - Examine retention by city.

### Predictive Modeling

1. **Feature Selection**:
   - Use relevant features such as city, phone, average distance, etc.

2. **Model Selection**:
   - Logistic Regression.
   - Random Forest.
   - Gradient Boosting.

3. **Evaluation Metrics**:
   - Accuracy, precision, recall, and F1-score.

4. **Model Performance**:
   - Gradient Boosting performed best with an accuracy of 0.78.

### Leveraging Insights

1. **Targeted Promotions**: Offer promotions in cities with lower retention rates.
2. **Incentives for First 30 Days**: Encourage more trips initially.
3. **Feedback and Support**: Enhance mechanisms for users with lower ratings.
4. **Ultimate Black Users**: Consider special programs for these users.

## Conclusion

This project provided valuable insights into user login patterns, designed an effective experiment to encourage cross-city driver participation, and built a predictive model to improve rider retention. These findings and recommendations can help Ultimate optimize their operations and enhance user satisfaction.

---

### Note

- Ensure to install necessary libraries: `pandas`, `matplotlib`, `seaborn`, `sklearn`.
- Clean up the dataset and delete any sensitive information after analysis.
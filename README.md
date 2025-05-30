# dsa210-project

# Screen Time, Stress, and Mood Analysis

## Project Background

Worries regarding the potential impacts of extended screen exposure on mental wellbeing have emerged due to our dramatic rise in dependence on smartphones in today’s digital age. This project examines the connection between everyday screen time and individually reported stress and mood changes. The research investigates whether spending more time on screens is linked to heightened stress levels and lower overall mood contentment by combining data obtained from Apple Screen Time with mood and stress information from apps like Daylio and Moodnotes.

## Project Objectives

* **Analyze Daily Screen Time:**
  Assess overall screen time, app-specific usage data, and the frequency of device unlocks based on reports produced by the Apple Screen Time feature.

* **Assess Psychological Well-Being:**
  Examine the daily stress levels and mood assessments that individuals report via Daylio and Moodnotes, offering an in-depth perspective on indicators of mental well-being.

* **Examine Relationships:**
  Determine the correlation between excessive screen time and elevated stress, as well as its potential impact on overall mood.

* **Generate Practical Recommendations:**
  Utilize the findings to present evidence-based suggestions aimed at enhancing screen time management and fostering better mental health.

## Data Sources

1. **Screen Time Data:**

   * **Source:**

     * Apple Screen Time application

   * **Metrics Collected:**

     * Total daily screen time
     * Breakdown of usage by app or category
2. **Stress and Mood Data:**

   * **Sources:**

     * Daylio: Provides daily logs of mood and stress levels, usually recorded on a numerical scale.
     * Moodnotes: Provides more information on mood monitoring and personal evaluation, classifying mood into positive, neutral, or negative categories.

## Hypothesis

**Hypothesis:**
"Excessive smartphone screen time is associated with increased stress levels and a deterioration in overall mood."

This theory suggests that as individuals devote more time to their smartphones, there will be a notable increase in stress levels and a clear deterioration in the quality of their mood.

## Data Collection and Preparation

### Data Collection

* **Screen Time Data:**
  Daily reports are exported from the Apple Screen Time app. These reports provide quantitative measures of smartphone usage in CSV format.

* **Stress and Mood Data:**
  Daily self-reports are gathered from Daylio and Moodnotes. These reports include both numerical stress ratings and categorical mood evaluations.

* **Data Integration:**
  The data sets are combined according to the date, making certain that the screen time statistics for each day correspond with the related entries for stress and mood.

### Data Preparation

* **Cleaning and Standardization:**

  * Convert date and time information into a consistent format (e.g., YYYY-MM-DD).
  * Identify and handle missing or inconsistent entries.
  * Remove or address outliers that may skew the analysis.

* **Feature Engineering:**

  * Create derived metrics such as "High Screen Time Days" versus "Low Screen Time Days" based on predefined thresholds.
  * Categorize days by time segments (e.g., morning, afternoon, evening) if detailed analysis by time of day is desired.

* **Data Alignment:**
  Ensure that the merged dataset is chronologically ordered, allowing for seamless analysis of trends over time.

## Exploratory Data Analysis (EDA)

### Descriptive Statistics

* **Screen Time Metrics:**

  * Compute mean, median and range of daily screen time.

* **Psychological Metrics:**

  * Calculate the average stress level and distribution of mood ratings.
  * Compare variations in stress and mood between days with high and low screen time.

### Visualization Techniques

* **Trend Analysis:**

  * Use line charts to display changes in screen time and corresponding stress/mood metrics over days or weeks.

* **Distribution Analysis:**

  * Generate histograms and box plots to visualize the distribution of screen time, stress scores, and mood ratings.

* **Correlation Visualizations:**

  * Create scatter plots and heatmaps to visually assess the strength and direction of relationships between screen time and psychological measures.

## Statistical Analysis

### Correlation Analysis

* **Method:**
  Compute Pearson's correlation coefficients to quantitatively assess the relationships between screen time, stress levels, and mood ratings.

* **Expected Outcome:**
  A direct link is expected to exist between the amount of time spent on screens and stress levels, whereas an inverse relationship is predicted between screen time and the quality of one’s mood.

### Regression Analysis

* **Linear Regression:**
  Develop regression models to predict stress and mood based on screen time data.

  * Analyze regression coefficients, R² values, and p-values to determine the predictive strength and significance of screen time metrics.

* **Hypothesis Testing:**
  Conduct t-tests to compare mean stress and mood scores on days with high screen time against those on days with low screen time, verifying whether the differences are statistically significant.

## Machine Learning (23 May Submission)

### Predictive Modeling

* Applied machine learning techniques (Random Forest Regressor, Linear Regression) to predict:

  * Daily stress scores
  * Daily mood scores

### Feature Transformation & Enrichment

* Transformed:

  * Screen time into categories: High vs. Low
  * Mood categories to ordinal numerical labels (Positive=3, Neutral=2, Negative=1)
* Enriched:

  * Added daily unlock frequency and app category usage where available

### Model Evaluation

* **Metrics Used:**

  * RMSE (Root Mean Squared Error)
  * R² Score
* **Findings:**

  * Random Forest slightly outperformed linear models in predicting both stress and mood.
  * Unlock frequency and app type usage had more predictive value than total screen minutes alone.

### Feature Importance

* Identified that productivity-related app usage is negatively associated with stress.
* Social media usage positively correlates with higher stress and lower mood scores.

## Final Findings and Recommendations (30 May Submission)

### Summary of Findings

* No strong linear correlation between screen time and stress/mood, but categorical insights suggest:

  * High screen time often coincides with higher stress (anecdotally)
  * Mood was more stable than stress, and more strongly influenced by app type than by total time

### Limitations

* Dataset consists of only 46 days and one user
* Self-reported mood and stress scores may carry subjective bias
* Limited external enrichment due to privacy restrictions

### Future Work

* Add more participants and scale the data across demographics
* Incorporate passive data collection for mood inference (e.g., voice, posture)
* Include time-of-day usage granularity
* Apply classification methods for stress/mood ranges instead of regression

## References

* Apple Screen Time: Primary source for quantitative smartphone usage data.
* Daylio: Mobile application for tracking daily mood and stress levels.
* Moodnotes: Additional tool for self-assessment and mood tracking.
* Academic literature and supporting sources referenced in the final report.

## Conclusion

This initiative examines the possible adverse effects of excessive smartphone usage on mental health. By employing comprehensive data gathering, thorough cleansing and organization, initial analysis, and statistical evaluation, the research confirms that while strong statistical relationships were not found, there are actionable trends. These include social media's correlation with negative mood and productivity app usage correlating with better outcomes. These findings contribute to the digital well-being discussion and support recommendations for healthier screen usage habits.

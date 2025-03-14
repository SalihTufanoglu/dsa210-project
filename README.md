# dsa210-project
# Screen Time, Stress, and Mood Analysis





## Project Background
Worries regarding the potential impacts of extended screen exposure on mental wellbeing have emerged due to our dramatic rise in dependence on smartphones in today’s digital age. This project examines the connection between everyday screen time and individually reported stress and mood changes. The study explores if increased screen usage correlates with elevated stress and a decrease in overall mood satisfaction by integrating data collected from Apple Screen Time alongside mood and stress records from applications such as Daylio and Moodnotes.


## Project Objectives
- *Analyze Daily Screen Time:
 Assess overall screen time, app-specific usage data, and the frequency of device unlocks based on reports produced by the Apple Screen Time feature.
  
- *Assess Psychological Well-Being:
 Examine the daily stress levels and mood assessments that individuals report via Daylio and Moodnotes, offering an in-depth perspective on indicators of mental well-being.

  
- **Examine Relationships:
  Determine the correlation between excessive screen time and elevated stress, as well as its potential impact on overall mood.
  
- **Develop Actionable Insights:
  Based on the analysis, offer data-driven recommendations to help optimize screen time usage and improve mental well-being.


## Data Sources
1. *Screen Time Data:
   - *Source:
     - Apple Screen Time application  
   - *Metrics Collected:
     - Total daily screen time
     - Breakdown of usage by app or category
      

2. *Stress and Mood Data:
   - *Sources:
     - *Daylio: Provides daily logs of mood and stress levels, usually recorded on a numerical scale.
     - *Moodnotes: Provides more information on mood monitoring and personal evaluation, classifying mood into positive, neutral, or negative categories.


## Hypothesis
*Hypothesis: 
"Excessive smartphone screen time is associated with increased stress levels and a deterioration in overall mood."  

This theory suggests that as individuals devote more time to their smartphones, there will be a notable increase in stress levels and a clear deterioration in the quality of their mood.


## Data Collection and Preparation
### Data Collection
- *Screen Time Data:
  Daily reports are exported from the Apple Screen Time app. These reports provide quantitative measures of smartphone usage in CSV format.
  
- *Stress and Mood Data:
  Daily self-reports are gathered from Daylio and Moodnotes. These reports include both numerical stress ratings and categorical mood evaluations.
  
- *Data Integration:
 The data sets are combined according to the date, making certain that the screen time statistics for each day correspond with the related entries for stress and mood.


### Data Preparation
- *Cleaning and Standardization:
  - Convert date and time information into a consistent format (e.g., YYYY-MM-DD).  
  - Identify and handle missing or inconsistent entries.  
  - Remove or address outliers that may skew the analysis.
  
- *Feature Engineering:
  - Create derived metrics such as "High Screen Time Days" versus "Low Screen Time Days" based on predefined thresholds.  
  - Categorize days by time segments (e.g., morning, afternoon, evening) if detailed analysis by time of day is desired.
  
- *Data Alignment:
  Ensure that the merged dataset is chronologically ordered, allowing for seamless analysis of trends over time.

## Exploratory Data Analysis (EDA)
### Descriptive Statistics
- *Screen Time Metrics:
  - Compute mean, median, standard deviation, and range of daily screen time.
  
- *Psychological Metrics:
  - Calculate the average stress level and distribution of mood ratings.  
  - Compare variations in stress and mood between days of high versus low screen time.

### Visualization Techniques
- **Trend Analysis:
  - Use line charts to display changes in screen time and corresponding stress/mood metrics over days or weeks.
  
- *Distribution Analysis:
  - Generate histograms and box plots to visualize the distribution of screen time, stress scores, and mood ratings.
  
- *Correlation Visualizations:
  - Create scatter plots and heatmaps to visually assess the strength and direction of relationships between screen time and psychological measures.

## Statistical Analysis
### Correlation Analysis
- *Method: 
  Compute Pearson's correlation coefficients to quantitatively assess the relationships between screen time, stress levels, and mood ratings.
  
- *Expected Outcome:
  A direct link is expected to exist between the amount of time spent on screens and stress levels, whereas an inverse relationship is predicted between screen time and the quality of        one’s mood.

### Regression Analysis
- *Linear Regression:
  Develop regression models to predict stress and mood based on screen time data.  
  - Analyze regression coefficients, R² values, and p-values to determine the predictive strength and significance of screen time metrics.
  
- *Hypothesis Testing:
  Conduct t-tests to compare mean stress and mood scores on days with high screen time against those on days with low screen time, verifying whether the differences are statistically         significant.

## Machine Learning
- *Predictive Modeling:
 Apply machine learning techniques such as Random Forest or Support Vector Regression to evaluate the influence of screen time on emotional well-being and stress levels.
  
- *Model Evaluation:
  Use performance metrics like RMSE (Root Mean Squared Error) and R² (Coefficient of Determination) to evaluate the accuracy of the predictive models.
  
- *Feature Importance:
  Examine how various screen time measurements (such as overall usage compared to the use of particular applications) influence fluctuations in stress and mood.

## Expected Outcomes and Discussion
- *Relationship Insights:
  The analysis is expected to reveal that higher screen time is significantly associated with increased stress levels and a decline in overall mood.
  
- *Practical Recommendations:
  According to the results, the initiative will recommend actionable approaches for regulating screen usage—like establishing daily thresholds or planning times free from screens—to          enhance psychological well-being.
  
- *Data-Driven Decisions:
  The research intends to lay the groundwork for additional investigation into online behaviors and their effects on mental health, which could shape individual lifestyle decisions as well   as wider digital health regulations.

## References
- *Apple Screen Time: Primary source for quantitative smartphone usage data.
- *Daylio: Mobile application for tracking daily mood and stress levels.
- *Moodnotes: Additional tool for self-assessment and mood tracking.
- Additional academic literature and online resources will be cited in the final report as necessary to support the analysis.

## Conclusion
This initiative examines the possible adverse effects of excessive smartphone usage on mental health. By employing comprehensive data gathering, thorough cleansing and organization, initial analysis, and statistical evaluation, the research seeks to confirm the theory that greater screen time is linked to elevated stress and diminished mood. The findings from this examination will inform suggestions for more beneficial digital practices and enhance the overall comprehension of digital well-being.

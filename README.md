# TikTok Data Analytics Project

## **Overview**

This project analyzes TikTok data to uncover trends, evaluate user engagement, and provide insights into content performance. Using Python and advanced analytics techniques, the project identifies factors driving virality and audience interaction on the platform.

## **Objectives**

- Analyze content performance metrics like views, likes, shares, and comments.
- Identify trends in popular hashtags, genres, and user engagement.
- Provide actionable insights to optimize TikTok content strategies.

## **Key Features**

- **Content Performance Analysis**: Evaluates metrics such as likes, shares, and comments to assess virality.
- **Trend Analysis**: Identifies popular hashtags and content categories.
- **User Engagement Insights**: Examines patterns in audience interactions over time.
- **Visualization**: Provides interactive charts and graphs for a comprehensive analysis.

## **Technologies Used**

- **Python**: Main language for data analysis.
- **Libraries**:
  - `Pandas` and `NumPy`: Data manipulation and preprocessing.
  - `Matplotlib` and `Seaborn`: Visualization.
  - `Plotly`: Interactive visualizations.
  - `Jupyter Notebook`: Interactive environment for data exploration.

## **Dataset Information**

- The dataset includes:
  - Video metrics (views, likes, shares, comments).
  - Hashtags and content genres.
  - Posting times and user demographics.

## **Steps to Reproduce**

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/AnalyticJosh/TikTok-Data-Analytics-Project.git
   cd TikTok-Data-Analytics-Project
   ```

2. **Set Up the Environment**:

   - Ensure Python (3.7 or higher) is installed.
   - Install required libraries:
     ```bash
     pip install -r requirements.txt
     ```

3. **Run the Notebook**:

   - Open `TikTok Project.ipynb` in Jupyter Notebook.
   - Execute cells sequentially to preprocess data, analyze trends, and visualize findings.

## **Sample Analysis**

### Engagement Rate Calculation

```python
data['EngagementRate'] = (data['Likes'] + data['Comments'] + data['Shares']) / data['Views'] * 100
```

### Popular Hashtags Analysis

```python
data['HashtagFrequency'] = data['Hashtags'].str.split(',').apply(len)
most_popular = data.explode('Hashtags')['Hashtags'].value_counts()
most_popular.head(10).plot(kind='bar', title='Top 10 Hashtags')
plt.show()
```

## **Results and Insights**

- Key findings:
  - Videos using trending hashtags received 30% higher engagement on average.
  - Content posted during peak hours (6–9 PM) performed significantly better in views and shares.
  - Dance and comedy genres dominated engagement metrics.
- Suggested strategies:
  - Leverage trending hashtags for improved visibility.
  - Schedule content releases during peak engagement times.
  - Focus on high-performing genres while experimenting with new trends.

## **Visualizations**

- **Engagement Trends**: Line chart showing interaction rates over time.
- **Top Hashtags**: Bar chart of most frequently used hashtags.
- **Content Genre Performance**: Pie chart illustrating distribution of views by genre.

## **Contributions**

Contributions are welcome! To contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-name`).
3. Commit your changes (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature-name`).
5. Open a Pull Request.

## **License**

This project is licensed under the MIT License.

---

For further inquiries or feedback, please contact [Joshua Amusan](mailto\:joshuaanalyst2@gmail.com).


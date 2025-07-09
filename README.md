# World Happiness Dashboard

This repository contains a data visualization project focused on exploring global happiness trends and the factors influencing them, utilizing the comprehensive World Happiness Report dataset. The project involves data loading, cleaning, analysis, and the creation of various static and interactive visualizations.

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Setup and Usage](#setup-and-usage)
- [Interactive Dashboard](#interactive-dashboard)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

The primary goal of this project is to visualize and analyze the World Happiness Report data to identify patterns, correlations, and trends in happiness scores across different countries and over the years. Various plots are generated, including scatter plots, bar charts, line charts, choropleth maps, and a correlation heatmap. An interactive dashboard is also created to allow users to explore the data dynamically.

## Dataset

The core of this project is the **World Happiness Report dataset**, which includes various indicators such as:
- Country name
- Year
- Life Ladder (happiness score)
- Log GDP per capita
- Social support
- Healthy life expectancy at birth
- Freedom to make life choices
- Generosity
- Perceptions of corruption
- Positive affect
- Negative affect

The dataset is loaded from a CSV file named `world-happiness-report (1).csv`.

## Features

- Data loading and initial exploration.
- Column standardization for easier analysis.
- **Static Visualizations:**
    - Distribution of Happiness Score Across Countries
    - Top and Bottom 10 Happiest Countries by Life Ladder Score
    - Correlation between Happiness and various indicators (e.g., Log GDP per Capita, Social Support)
    - Happiness Trends for Top 5 Countries over recent years
    - Relationship between Log GDP per Capita and Happiness
    - Happiness Score Distribution by Continent (Box Plot and Bar Chart)
    - Feature Contribution to Happiness Score (using Linear Regression)
    - Happiness vs. Corruption Perception
    - Trend of Happiness Over Time
- **Interactive Visualizations:**
    - Choropleth map of Happiness Score Across Countries.
    - 2D and 3D Clustering of Countries Based on Happiness Factors (GDP per capita, Social Support, Healthy Life Expectancy).
    - Global Happiness Trend Over the Last Five Years (animated choropleth).
    - Interactive Altair dashboard of Top and Bottom 10 Happiest Countries.

## Technologies Used

- Python
- Pandas (for data manipulation and analysis)
- NumPy (for numerical operations)
- Matplotlib (for static visualizations)
- Seaborn (for enhanced statistical visualizations)
- Altair (for declarative statistical visualizations and interactive dashboard creation)
- Plotly Express (for interactive visualizations like choropleth maps and 3D scatter plots)
- Scikit-learn (for machine learning models like Linear Regression and KMeans clustering)
- Google Colab (for environment setup and execution)

## Setup and Usage

To run this project:

1.  **Clone the repository (or download the `data_visualization_final_project_(ph) (1).py` file):**

    ```bash
    git clone [https://github.com/YourUsername/World-Happiness-Dashboard.git](https://github.com/YourUsername/World-Happiness-Dashboard.git)
    cd World-Happiness-Dashboard
    ```

2.  **Ensure you have the dataset:**
    The script expects the `world-happiness-report (1).csv` dataset. The notebook version of this project typically loads it from Google Drive. If running locally, place the CSV file in the same directory as the Python script, or update the `pd.read_csv` path in the script:

    ```python
    df = pd.read_csv('/path/to/your/dataset/world-happiness-report (1).csv')
    ```

3.  **Install necessary libraries:**
    You can install the required Python libraries using pip:

    ```bash
    pip install pandas numpy matplotlib seaborn altair plotly scikit-learn
    ```

4.  **Run the Python script:**

    ```bash
    python data_visualization_final_project_(ph) (1).py
    ```
    This will generate various static plots and open interactive Plotly visualizations in your default browser.

## Interactive Dashboard

An interactive Altair dashboard is generated and, when run in an environment like Google Colab, is typically saved as `interactive_happiness_profile_final.json`.

To view and interact with the Altair dashboard:

1.  If running in Google Colab, after executing the relevant cells, download `interactive_happiness_profile_final.json` from the 'Files' tab (the folder icon on the left sidebar).
2.  Open this JSON file in a Vega-Lite viewer (e.g., [Vega-Lite Online Editor](https://vega.github.io/vega-lite/examples/)).
    This will allow you to interact with the dashboard, filter data, and explore different aspects of global happiness.

## Contributing

Feel free to fork this repository, contribute, and suggest improvements.

## License

This project is open-source and available under the MIT License.

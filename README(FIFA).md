# FIFA World Cup Data Analysis

This project explores and analyzes FIFA World Cup data from various datasets, including match results, player statistics, and tournament details. The analysis covers key insights like goals scored over the years, top teams and players, attendance trends, and more.

## Table of Contents

- [Introduction](#introduction)
- [Datasets](#datasets)
- [Project Workflow](#project-workflow)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Feature Engineering](#feature-engineering)
- [Modeling](#modeling)
- [Data Visualization](#data-visualization)
- [Installation](#installation)
- [Results](#results)
- [Future Work](#future-work)
- [Contributing](#contributing)
- [License](#license)

## Introduction

This project leverages FIFA World Cup data to uncover patterns and insights about the tournament’s history, team performance, player statistics, and attendance. The dataset is analyzed with Python and visualized using libraries such as Matplotlib and Seaborn.

## Datasets

The project includes the following datasets:

- **WorldCups.csv**: Contains historical data on FIFA World Cup tournaments, including year, winning team, goals scored, and attendance.
- **WorldCupMatches.csv**: Provides match-level data, including date, teams, stage, and goals scored.
- **WorldCupPlayers.csv**: Contains player-level data for each match, including player name, team, and position.

## Project Workflow

1. **Data Loading and Cleaning**: Loading datasets, handling missing values, and cleaning the data.
2. **Exploratory Data Analysis (EDA)**: Analyzing goals scored, team performance, match stages, and attendance.
3. **Feature Engineering**: Creating new features like decade and era.
4. **Data Visualization**: Visualizing key insights.
5. **Modeling**: Basic Random Forest model for feature importance.
6. **Saving Cleaned Data**: Saving cleaned datasets for future use.

## Exploratory Data Analysis (EDA)

### Goals Scored Over the Years
A line plot visualizes the total goals scored each World Cup year.

### Top Teams and Players
- Bar charts identify the teams with the most World Cup wins.
- Analysis of top players by the number of appearances.

### Attendance Trends
A line plot shows the attendance over the years, helping to identify trends in audience engagement.

## Feature Engineering

We created new categorical features:
- **Decade**: Groups each tournament into a decade.
- **Era**: Classifies each tournament as *Early*, *Mid*, or *Modern* based on the year.

## Modeling

Using a RandomForestClassifier, we analyzed feature importance in predicting outcomes. This step highlights which features are most influential.

## Data Visualization

The project includes visualizations such as:
- Line plots for goals scored and attendance trends
- Bar charts for team and player analysis
- Box plots for match outcomes by stage

## Installation

1. Clone this repository.
   ```bash
   git clone https://github.com/yourusername/FIFA-WorldCup-Analysis.git
2. Install the required libraries
    pip install -r requirements.txt
## Results

Key insights from this analysis include:

- Patterns in goals scored and attendance.
- Dominant teams and players across World Cup history.
- Influential match stages on home and away goals.

## Future Work

Future enhancements to the project may include:

- More complex machine learning models.
- In-depth player performance analysis.
- Predictive modeling on team performances.

## Contributing

Contributions are welcome! Please submit a pull request or open an issue if you have suggestions for improvement.

## License

This project is licensed under the MIT License.

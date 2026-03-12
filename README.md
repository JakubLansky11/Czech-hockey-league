# Czech-hockey-league---data-analysis
Analysis of data from Czech hockey league (Tipsport Extraliga) - players and teams statistics

# Czech Extraliga Hockey Analytics Dashboard

This project analyzes data from the Czech ice hockey league (Tipsport Extraliga) and presents interactive team and player statistics using Power BI.

The dashboard allows users to compare teams across multiple seasons and explore player performance, scoring patterns, and team results.

## Project Overview

The goal of this project was to practice data analysis and visualization on a real dataset from a topic I am interested in – ice hockey.

The project focuses on:

- collecting and transforming sports data
- building a structured data model
- creating an interactive Power BI dashboard
- comparing teams and player performance across multiple seasons

The dataset currently contains **12 seasons of Czech Extraliga data (2014/15 – present)**.

---

# Data Collection

Data was collected using **Power Query** directly from publicly available tables of the Czech Extraliga.

Two types of data were collected:

- league standings (regular season tables)
- player statistics

The workflow was:

1. Import the standings table for one season using Power Query.
2. Clean and transform the data.
3. Duplicate the query and modify the source to import the next season.
4. Repeat this process for all seasons.
5. Apply the same approach for player statistics.

This allowed me to quickly collect and combine data from multiple seasons using a consistent structure.

---

# Data Transformation

Data preparation was done mainly in **Power Query**.

Steps included:

- cleaning column names
- removing unnecessary columns
- ensuring consistent column structure across seasons
- appending multiple seasons into a single dataset
- preparing tables for use in Power BI

The final dataset includes:

- team statistics per season
- player statistics per season
- scoring statistics (goal types)
- season identifiers

---

# Data Model

The Power BI model uses a **star schema approach** with fact tables and dimension tables.

Main tables:

Fact tables:
- team season statistics
- player statistics

Dimension tables:
- teams
- seasons

Additional disconnected tables were created for interactive comparisons:

- Team A
- Team B

These tables allow the user to compare two teams dynamically within the dashboard.

---

# Dashboard Features

The Power BI dashboard includes:

### Team comparison
Compare two teams across selected seasons.

### Team performance metrics
- total points
- wins
- overtime wins
- overtime losses
- regulation losses
- goals scored
- goals conceded

### Season trends
Line charts showing team performance across seasons.

### Goal type analysis
Breakdown of goals scored:
- even strength
- power play
- shorthanded

### Player statistics
Tables showing top players from selected teams:
- goals
- assists
- total points
- game-winning goals

---

# Tools Used

- **Power Query** – data extraction and transformation  
- **Power BI** – data modeling and dashboard creation  
- **DAX** – measures and calculations  
- **GitHub** – project repository and documentation  

---

# Example Questions This Dashboard Can Answer

- Which team performed better across selected seasons?
- How did teams evolve over time?
- Which players had the highest scoring seasons?
- How do teams score their goals (even strength vs power play)?
- Which teams rely more on special teams?

---

# Project Motivation

This project combines two of my interests:

- data analysis
- ice hockey

By working with real sports data, I was able to practice building a full analytics workflow including data collection, transformation, modeling, and visualization.

---

# Future Improvements

The project will be extended with additional data analysis and automation steps.

Planned improvements include:

- Performing deeper statistical analysis using **Python** (pandas, matplotlib, seaborn).
- Writing **SQL scripts** for more advanced queries and data exploration.
- Creating additional metrics such as team efficiency, scoring trends, and player performance indicators.
- Automating data collection and updates for new seasons.
- Expanding the dataset with more seasons and potentially playoff statistics.

# Skill demonstrated

- Power Query data extraction
- Data cleaning and transformation
- Star schema data modeling
- DAX measures
- Interactive dashboard design
- Sports data analysis

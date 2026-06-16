# 🏏 IPL 2024 Data Analysis using PySpark

A comprehensive data engineering project analyzing Indian Premier League (IPL) 2024 cricket tournament data using Apache PySpark, SQL, and Jupyter Notebooks.

---

## 📋 Table of Contents

- [Project Overview](#-project-overview)
- [Objectives](#-objectives)
- [Data Model](#-data-model)
- [Project Structure](#-project-structure)
- [Notebooks Description](#-notebooks-description)
- [Technologies Used](#-technologies-used)
- [Key Features](#-key-features)
- [How to Use](#-how-to-use)
- [Insights & Analysis](#-insights--analysis)
- [Getting Started](#-getting-started)

---

## 🎯 Project Overview

This project demonstrates practical data engineering and analytics capabilities by analyzing comprehensive IPL 2024 tournament data. The project involves:

- **Data Ingestion**: Loading IPL 2024 cricket data from official IPL source (https://www.iplt20.com/match/2024/1354)
- **Data Transformation**: Using PySpark for large-scale data processing and SQL for complex queries
- **Data Modeling**: Creating normalized database schema with proper relationships
- **Analysis**: Generating insights about match performance, batting statistics, and bowling performance

This is an end-to-end project that showcases ETL (Extract, Transform, Load) pipeline development and data analytics best practices.

---

## 🎯 Objectives

✅ **Data Integration**: Combine and clean raw IPL 2024 cricket data  
✅ **Schema Design**: Create a normalized relational database model  
✅ **Performance Analysis**: Analyze batting and bowling statistics  
✅ **Match Insights**: Generate comprehensive match summary reports  
✅ **PySpark Proficiency**: Demonstrate distributed data processing capabilities  
✅ **SQL Expertise**: Write complex queries for data extraction and analysis  

---

## 📊 Data Model

### Entity Relationship Diagram (ERD)

![IPL 2024 ER Diagram](IPL_2024_ER.png)

### Core Tables

| Table | Description |
|-------|-------------|
| **Teams** | IPL franchise information and team details |
| **Matches** | Match metadata including venue, date, and result |
| **Innings** | Innings-level data for each match |
| **Batsmen** | Individual batsman statistics and performance |
| **Bowlers** | Individual bowler statistics and performance |
| **Ball_by_Ball** | Granular ball-level data including runs, wickets, and deliveries |

---

## 📁 Project Structure

```
Pyspark_Project_IPL_2024/
│
├── README.md                           # Project documentation (this file)
├── IPL_2024_ER.png                     # Entity Relationship Diagram
│
└── Pyspark_IPL_2024/                   # Main project directory
    │
    ├── 1. Create all tables.ipynb      # Database table creation & data loading
    ├── 2. Match Summary.ipynb          # Match-level analysis and insights
    ├── 3. Batting Scorecard.ipynb      # Batting statistics and performance
    ├── 5. Bowling Scorecard.ipynb      # Bowling statistics and performance
    │
    └── image_*.png                     # Analysis visualizations & charts
```

---

## 📓 Notebooks Description

### **1. Create all tables.ipynb** 🗂️
**Purpose**: Database Initialization & Data Loading

This notebook handles the foundational setup of the entire project:

- **Data Source Integration**: Loads raw IPL 2024 cricket data from CSV/Parquet files
- **PySpark Session Initialization**: Sets up Spark environment and configurations
- **Schema Definition**: Creates DataFrames with proper data types and constraints
- **Table Creation**: Generates normalized tables following the ER model:
  - Teams table (team information)
  - Matches table (match metadata)
  - Innings table (inning details)
  - Batsmen table (batting records)
  - Bowlers table (bowling records)
  - Ball_by_Ball table (granular match events)
- **Data Validation**: Performs quality checks and data cleansing
- **Data Persistence**: Saves processed data in optimized formats (Parquet)

**Key Outputs**: Clean, normalized database tables ready for analysis

---

### **2. Match Summary.ipynb** 🎯
**Purpose**: Match-Level Analysis & Comprehensive Insights

Provides high-level tournament and match analytics:

- **Match Overview**: Summary of all matches played in IPL 2024
- **Tournament Statistics**:
  - Total matches played
  - Number of teams
  - Venues used
  - Date range of tournament
- **Match-wise Insights**:
  - Win/loss patterns
  - Toss decisions and outcomes
  - Winning margins (runs/wickets)
  - Super Over information (if any)
- **Team Performance**:
  - Matches won by each team
  - Win percentage
  - Head-to-head records
- **Venue Analysis**:
  - Matches per venue
  - Average scores by venue
  - Home advantage statistics
- **Visualizations**: Charts showing tournament trends and patterns

**Key Outputs**: Tournament overview, team performance metrics, match statistics

---

### **3. Batting Scorecard.ipynb** 🏏
**Purpose**: Batting Performance Analysis & Individual Statistics

Detailed analysis of batting performances throughout the tournament:

- **Individual Batsman Performance**:
  - Runs scored (total, per match average)
  - Strike rate calculations
  - Batting average
  - Number of innings played
  - Highest individual score
  - Half-centuries and centuries
- **Aggregated Statistics**:
  - Runs by batsman (top performers)
  - Runs by team
  - Runs by venue
- **Performance Metrics**:
  - Consistency analysis
  - Best performances in specific conditions
  - Performance against specific teams
- **Comparative Analysis**:
  - Top run-scorers
  - Best strike rates
  - Most consistent performers
- **Visualizations**:
  - Top scorers ranking
  - Strike rate distribution
  - Performance trends

**Key Outputs**: Batting statistics, player performance metrics, ranking tables

---

### **5. Bowling Scorecard.ipynb** 🎲
**Purpose**: Bowling Performance Analysis & Bowler Statistics

Comprehensive analysis of bowling performances:

- **Individual Bowler Performance**:
  - Wickets taken (total, per match average)
  - Economy rate (runs per over)
  - Bowling average
  - Number of matches bowled
  - Best bowling figures
  - 4-wicket hauls and 5-wicket hauls
- **Aggregated Statistics**:
  - Wickets by bowler (top performers)
  - Wickets by team
  - Wickets by venue
- **Performance Metrics**:
  - Dot ball percentages
  - Death bowling analysis
  - Performance against left/right-handed batsmen
- **Comparative Analysis**:
  - Top wicket-takers
  - Best economy rates
  - Most economical bowlers
- **Visualizations**:
  - Top wicket-takers ranking
  - Economy rate trends
  - Bowling performance charts

**Key Outputs**: Bowling statistics, bowler rankings, efficiency metrics

---

## 🛠️ Technologies Used

| Technology | Purpose |
|-----------|---------|
| **Apache PySpark** | Distributed data processing and big data analytics |
| **Python 3.x** | Programming language for data manipulation |
| **Jupyter Notebook** | Interactive development and documentation |
| **SQL** | Querying and data analysis |
| **Pandas** | Data manipulation and transformation |
| **Matplotlib/Seaborn** | Data visualization and charting |
| **CSV/Parquet** | Data storage formats |

---

## ✨ Key Features

🔹 **Complete ETL Pipeline**: End-to-end data processing from raw data to insights  
🔹 **Normalized Database Schema**: Properly designed relational model with ERD  
🔹 **PySpark Distributed Processing**: Handles large-scale data efficiently  
🔹 **SQL Analytics**: Complex queries for detailed data extraction  
🔹 **Comprehensive Analysis**: Batting, bowling, and match-level insights  
🔹 **Data Visualization**: Multiple charts and visualizations for easy understanding  
🔹 **Jupyter Notebooks**: Interactive, well-documented code with markdown explanations  
🔹 **Reproducible**: Clear step-by-step pipeline for easy replication  

---

## 📖 How to Use

### Prerequisites
```bash
# Install required Python packages
pip install pyspark pandas jupyter matplotlib seaborn
```

### Running the Project

1. **Clone the Repository**
   ```bash
   git clone https://github.com/Rupam-1/Pyspark_Project_IPL_2024.git
   cd Pyspark_Project_IPL_2024
   ```

2. **Start Jupyter Notebook**
   ```bash
   jupyter notebook
   ```

3. **Execute Notebooks in Order**
   - Open `Pyspark_IPL_2024/1. Create all tables.ipynb` - Sets up all tables
   - Open `Pyspark_IPL_2024/2. Match Summary.ipynb` - View tournament overview
   - Open `Pyspark_IPL_2024/3. Batting Scorecard.ipynb` - Analyze batting stats
   - Open `Pyspark_IPL_2024/5. Bowling Scorecard.ipynb` - Analyze bowling stats

4. **Run Each Cell**: Execute cells sequentially to process data and generate insights

---

## 📊 Insights & Analysis

### Sample Questions Answered

**Tournament Level**:
- How many matches were played in IPL 2024?
- Which team won the most matches?
- What was the average margin of victory?

**Batting Analysis**:
- Who was the top run-scorer in IPL 2024?
- What were the highest strike rates?
- How many half-centuries and centuries were scored?

**Bowling Analysis**:
- Who took the most wickets?
- Which bowler had the best economy rate?
- What were the best bowling figures?

**Performance Metrics**:
- How did teams perform at different venues?
- What was the impact of winning the toss?
- Which venues had the highest average scores?

---

## 🚀 Getting Started

### Quick Start
```python
# Example: Load and explore match data
from pyspark.sql import SparkSession

spark = SparkSession.builder.appName("IPL2024").getOrCreate()
matches_df = spark.read.parquet("path/to/matches.parquet")
matches_df.show()
```

### Next Steps
1. Review the ER diagram (`IPL_2024_ER.png`) to understand data structure
2. Start with Notebook 1 to set up the database
3. Explore each analysis notebook for specific insights
4. Modify queries to answer custom questions

---

## 📈 Project Highlights

✅ **Data Processing**: Handled large-scale cricket data with PySpark  
✅ **Schema Design**: Created normalized, efficient database schema  
✅ **Analysis Depth**: Provided multi-level analysis (tournament, team, individual)  
✅ **Documentation**: Comprehensive notebooks with markdown explanations  
✅ **Visualizations**: Multiple charts for easy data interpretation  
✅ **Reproducibility**: Clear, step-by-step pipeline for easy replication  

---

## 📝 Notes

- The project uses IPL 2024 official tournament data
- All analysis is based on standardized cricket metrics
- Data is processed in normalized form for consistency
- Visualizations are generated dynamically from the data

---

## 🤝 Contributing

If you'd like to extend this project:
- Add more analysis notebooks
- Enhance visualizations
- Incorporate additional data sources
- Optimize query performance

---

## 📧 Contact & Support

For questions or suggestions regarding this project, feel free to reach out.

---

## 📄 License

This project is open source and available under the MIT License.

---

**Last Updated**: June 2026  
**Project Status**: ✅ Complete & Documented

---

### 🙏 Acknowledgments

This project demonstrates practical applications of:
- Apache PySpark for distributed data processing
- SQL for data querying and analysis
- Data engineering best practices
- Cricket analytics using real IPL 2024 data

---

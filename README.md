# Netflix Dataset Analysis Project

## 📋 Project Overview

This project provides a comprehensive analysis of Netflix's content catalog, examining 8,807 titles to extract valuable business insights and strategic recommendations. The analysis covers content distribution, geographic patterns, release timing, talent analysis, and genre trends.

## 🎯 Objectives

- Analyze Netflix's content portfolio composition
- Identify geographic content distribution patterns
- Determine optimal release timing strategies
- Examine top talent and genre preferences
- Provide actionable business recommendations

## 📊 Dataset Information

- **Total Records**: 8,807 Netflix titles
- **Time Period**: 1925-2021 (96 years)
- **Content Types**: Movies (69.6%) and TV Shows (30.4%)
- **Geographic Coverage**: 123 countries
- **Genre Diversity**: 42 unique genres

### Dataset Columns:
- `show_id`: Unique identifier
- `type`: Movie or TV Show
- `title`: Content title
- `director`: Director(s)
- `cast`: Main cast members
- `country`: Production country(ies)
- `date_added`: Date added to Netflix
- `release_year`: Original release year
- `rating`: Content rating (TV-MA, PG-13, etc.)
- `duration`: Runtime (minutes for movies, seasons for TV shows)
- `listed_in`: Genres/categories
- `description`: Content description

## 🚀 Quick Start

### Prerequisites
```bash
Python 3.7+
pandas
numpy
matplotlib
seaborn
wordcloud (optional)
```

### Installation
1. **Clone or download** this project
2. **Install required packages**:
   ```bash
   pip install pandas numpy matplotlib seaborn wordcloud
   ```
3. **Ensure `netflix.csv`** is in the project directory

### Running the Analysis

#### Option 1: Run Complete Analysis Script
```bash
python run_netflix_analysis.py
```

#### Option 2: Use Jupyter Notebook
1. Open `netflix_analysis_complete.ipynb`
2. Run cells sequentially
3. Add additional sections from `netflix_analysis_part2.py`

#### Option 3: Generate Visualizations
```bash
python create_visualizations.py
```

## 📁 Project Structure

```
netflix-analysis/
├── README.md                           # This file
├── netflix.csv                         # Dataset (required)
├── run_netflix_analysis.py            # Main analysis script
├── netflix_analysis_complete.ipynb    # Jupyter notebook
├── netflix_analysis_part2.py          # Additional analysis sections
├── netflix_insights_recommendations.py # Business recommendations
├── create_visualizations.py           # Visualization generator
├── netflix_analysis_visualizations.png # Generated charts
├── netflix_final_report.md            # Comprehensive report
├── fix_imports.py                      # Import helper
└── setup_environment.py               # Environment checker
```

## 🔍 Analysis Components

### 1. Data Preprocessing
- **Null Value Handling**: Categorical → "Unknown_ColumnName", Numerical → 0
- **Data Un-nesting**: Split comma-separated values (cast, country, genres)
- **Data Cleaning**: Standardize formats and remove inconsistencies

### 2. Categorical Analysis
- **Non-graphical**: Value counts for all categorical variables
- **Graphical**: Count plots, bar charts, pie charts

### 3. Geographic Analysis
- **Movies by Country**: Top 10 countries for movie production
- **TV Shows by Country**: Top 10 countries for TV show production
- **Content Distribution**: Global reach and regional preferences

### 4. Temporal Analysis
- **Release Timing**: Best weeks and months for content releases
- **Seasonal Patterns**: Identify peak release periods
- **Acquisition Timeline**: Time from release to Netflix addition

### 5. Talent Analysis
- **Top Directors**: Most prolific directors by title count
- **Top Actors**: Most featured actors across content
- **Collaboration Patterns**: Frequent director-actor partnerships

### 6. Genre Analysis
- **Popularity Rankings**: Most common genres
- **Word Cloud Visualization**: Genre frequency representation
- **Content Categorization**: Genre distribution patterns

## 📈 Key Findings

### Content Portfolio
- **Movies**: 6,131 titles (69.6%)
- **TV Shows**: 2,676 titles (30.4%)
- **Content Freshness**: 70.6% released since 2015

### Geographic Distribution
1. **United States**: 3,690 titles (41.9%)
2. **India**: 1,046 titles (11.9%)
3. **United Kingdom**: 806 titles (9.2%)
4. **Canada**: 445 titles (5.1%)
5. **France**: 393 titles (4.5%)

### Release Timing
- **Peak Months**: July (819), December (797), September (765)
- **Optimal Strategy**: Summer and holiday season releases

### Top Talent
- **Most Featured Actor**: Anupam Kher (43 titles)
- **Most Prolific Director**: Rajiv Chilaka (22 titles)

### Genre Preferences
1. **International Movies**: 2,752 titles
2. **Dramas**: 2,427 titles
3. **Comedies**: 1,674 titles

## 💡 Business Recommendations

### Content Strategy
- **Balance Portfolio**: Increase TV show production to 40% of catalog
- **Focus on Series**: TV shows acquired faster (632 vs 869 days)
- **Maintain Freshness**: Continue emphasis on recent content

### Geographic Expansion
- **Strengthen Asian Markets**: Beyond Japan and South Korea
- **Develop Latin America**: Build on Mexico foundation
- **European Diversification**: Expand beyond UK, France, Germany

### Release Optimization
- **Seasonal Planning**: Leverage July and December peaks
- **Content Calendar**: Coordinate global releases
- **Acquisition Timing**: Reduce movie acquisition timeline

### Talent Acquisition
- **Exclusive Partnerships**: High-output directors and actors
- **Regional Development**: Invest in local talent
- **Cross-Cultural Content**: International collaborations

## 🛠 Technical Details

### Data Processing
- **Missing Data**: 29.9% directors, 9.4% cast/country missing
- **Data Types**: Mixed categorical and numerical
- **Preprocessing**: Standardization and normalization

### Analysis Methods
- **Statistical Analysis**: Descriptive statistics, distributions
- **Data Visualization**: Multiple chart types and dashboards
- **Business Intelligence**: KPI development and tracking

### Performance Metrics
- **Content Freshness**: 70.6% (Target: 75%+)
- **International Diversity**: 58.1% (Target: 65%+)
- **Data Completeness**: 70.1% director info (Target: 85%+)

## 📊 Visualizations

The project generates comprehensive visualizations including:
- Content type distribution (pie chart)
- Geographic content mapping (bar charts)
- Temporal release patterns (line graphs)
- Genre popularity (word clouds)
- Talent analysis (ranking charts)
- Duration distributions (histograms)

## 🔧 Troubleshooting

### Common Issues

**Import Errors**:
```python
# Run this first in your notebook
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
```

**File Not Found**:
- Ensure `netflix.csv` is in the same directory
- Check file permissions and path

**Memory Issues**:
- Use data sampling for large datasets
- Close unnecessary applications

### Getting Help
1. Check the `fix_imports.py` file for import solutions
2. Run `setup_environment.py` to verify installation
3. Review error messages for specific issues

## 📝 Case Study Compliance

This project fulfills all requirements for Netflix case study analysis:
- ✅ Data preprocessing and null value handling
- ✅ Categorical variable analysis (graphical and non-graphical)
- ✅ Movies vs TV shows comparison by country
- ✅ Optimal release timing analysis
- ✅ Actor and director analysis
- ✅ Genre popularity insights
- ✅ Netflix addition timeline analysis
- ✅ Business recommendations and insights

## 🎓 Learning Outcomes

This project demonstrates:
- **Data Science Skills**: Cleaning, analysis, visualization
- **Business Intelligence**: Strategic insights and recommendations
- **Technical Proficiency**: Python, pandas, matplotlib, seaborn
- **Communication**: Clear reporting and presentation

## 📄 License

This project is for educational and analytical purposes. Dataset used under fair use for academic analysis.

## 👥 Contributing

Feel free to fork this project and submit improvements:
- Additional visualizations
- Enhanced analysis methods
- Extended business recommendations
- Code optimizations

---

**Created for Netflix Dataset Case Study Analysis**  
*Comprehensive data analysis with actionable business insights*


# TikTok_Engagement_Analysis
Exploratory analysis of TikTok engagement data focused on content classification, engagement behavior, outlier detection, and behavioral patterns using Python, Pandas, and statistical visualization techniques.

# TikTok Claim Analysis

This project presents an exploratory analysis of TikTok engagement data with a focus on content classification, user engagement behavior, author moderation status, and engagement-driven patterns across claim and opinion-based videos.

The analysis was conducted using Python, Pandas, Seaborn, and Matplotlib, following a structured exploratory data analysis workflow.

---

## Project Overview

The objective of this project is to investigate behavioral and engagement differences between claim videos and opinion videos within the TikTok dataset.

The analysis focuses on:

- Content engagement metrics
- Claim versus opinion content behavior
- Author ban status patterns
- Outlier detection and distribution analysis
- Relationships between engagement variables

---

## Dataset

Dataset used:

- `tiktok_dataset.csv`

The dataset contains information related to:

- Video duration
- View count
- Like count
- Share count
- Download count
- Comment count
- Claim status
- Author ban status

---

## Technologies Used

- Python
- Pandas
- Matplotlib
- Seaborn
- Quarto

---

## Workflow

### 1. Data Inspection and Validation

Performed initial dataset exploration using:

- `info()`
- `describe()`
- `shape`
- Missing value analysis

Handled missing values by identifying incomplete rows and removing null observations where appropriate.

---

### 2. Exploratory Data Analysis

Conducted distribution analysis on key numerical variables including:

- `video_duration_sec`
- `video_view_count`

Visualizations created:
- Histograms
- Boxplots

Additional automated visualization loops were created for all numerical features.

---

### 3. Claim Status Analysis

Analyzed relationships between:

- Claim status
- Author ban status
- Video engagement metrics

Visualizations included:

- Histogram of claim status by author ban status
- Median video view count comparisons
- Total view share distribution using pie charts

---

### 4. Outlier Detection

Applied the Interquartile Range (IQR) method to detect outliers across engagement metrics including:

- Video views
- Likes
- Shares
- Downloads
- Comments

---

### 5. Relationship Analysis

Created scatterplots to analyze relationships between:

- `video_view_count`
- `video_like_count`

Comparisons were performed for:
- All videos
- Opinion-only videos
- Claim versus opinion engagement behavior

---

## Key Findings

- A strong positive relationship exists between video views and likes.
- Claim videos consistently achieve higher engagement levels than opinion videos.
- Engagement-related variables exhibit heavy right-skewness with significant outlier presence.
- Engagement variability increases substantially for high-view videos.
- Author moderation status appears associated with differences in engagement patterns.

---

## Visualizations Included

The project includes:

- Histograms
- Boxplots
- Scatterplots
- Barplots
- Pie charts

used to analyze distributions, engagement behavior, and variable relationships.

---

## Project Structure

```text
├── TikTok_Claim_Analysis.qmd
├── tiktok_dataset.csv
├── README.md
└── TikTok_Claim_Analysis.html
```

---

## Installation

Install required dependencies:

```bash
pip install pandas matplotlib seaborn quarto
```

---

## Running the Project

Render the Quarto report:

```bash
quarto render TikTok_Claim_Analysis.qmd --to html
```

---

## Author

Udith P Kidiyoor

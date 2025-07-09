# 🍿 Project 6: Netflix User Behavior Analysis

## 📌 Problem Statement

Streaming platforms aim to optimize user satisfaction by understanding viewing preferences and behaviors. This project uses IMDb's Top 5000 TV Shows data as a proxy to analyze genre trends, show durations, and user engagement patterns.

---

## 🎯 Objective

- Identify the most popular genres.
- Analyze how show ratings relate to genres and vote counts.
- Explore binge behavior via show durations.
- Visualize how trends have evolved over the years.

---

## 📁 Dataset

- Source: IMDb Top 5000 TV Shows
- Columns Used:
  - `primaryTitle`
  - `startYear`, `endYear`
  - `averageRating`, `numVotes`
  - `genres`
  - `directors`, `writers`

---

## 📊 Exploratory Data Analysis & Visualizations

All plots are saved in the `images/` folder.

| Visualization | File |
|---------------|------|
| Top 10 Most Common Genres | `images/top_genres.png` |
| Top 10 Highest Rated Genres | `images/top_rated_genres.png` |
| Distribution of Average Ratings | `images/rating_distribution.png` |
| Distribution of Show Duration (Years) | `images/show_duration.png` |
| Top 15 Most Voted Shows | `images/top_voted_shows.png` |
| Rating vs Number of Votes (Colored by Duration) | `images/rating_vs_votes.png` |
| TV Shows Released Over the Years | `images/shows_by_year.png` |

---

## 🧠 Insights

- Certain genres like **Drama**, **Comedy**, and **Reality-TV** dominate in volume.
- Genres like **Documentary** and **History** tend to have higher average ratings.
- Most shows run for less than 10 years.
- A few shows accumulate extremely high votes, indicating strong user engagement.
- Ratings and vote counts have a moderate relationship, influenced by show duration.
- Content creation has surged since the early 2000s.

---


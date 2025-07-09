# 🎓 Student Performance Analytics Dashboard

## 📌 Problem Statement
Educational institutions often lack early warning systems to identify students at risk of failing or dropping out. Timely insights into performance metrics are essential for proactive academic interventions.

---

## 🎯 Objective
To build a data-driven dashboard that analyzes student-related parameters to:
- Highlight academic performance trends
- Identify at-risk students
- Support timely and personalized interventions

---

## 📂 Dataset Description

The dataset contains **6607 records** with the following columns:

| Feature | Description |
|--------|-------------|
| `Hours_Studied` | Number of hours studied per week |
| `Attendance` | Total attendance percentage |
| `Parental_Involvement` | High/Medium/Low involvement |
| `Access_to_Resources` | Availability of learning resources |
| `Extracurricular_Activities` | Participation in extracurriculars |
| `Sleep_Hours` | Average sleep hours per day |
| `Previous_Scores` | Last academic score |
| `Motivation_Level` | Self-reported motivation |
| `Internet_Access` | Yes/No |
| `Tutoring_Sessions` | No. of tutoring sessions attended |
| `Family_Income` | Income category |
| `Teacher_Quality` | Rated by student feedback |
| `School_Type` | Government/Private |
| `Peer_Influence` | Peer pressure or support |
| `Physical_Activity` | Hours per week |
| `Learning_Disabilities` | Yes/No |
| `Parental_Education_Level` | Education background of parents |
| `Distance_from_Home` | Distance to school |
| `Gender` | Male/Female |
| `Exam_Score` | Final exam score (Target Variable) |

---

## 🧪 Key Tasks Performed

- Handled missing values using mode imputation
- Performed descriptive statistics on key features
- Correlation analysis between numeric features
- Classified students into `Top`, `Average`, and `Struggling`
- Explored impacts of attendance, motivation, internet access, and sleep
- Created interactive and static visualizations

---

## 📊 Visualizations

- 📌 **Heatmap** of correlations between performance indicators  
- 📌 **Scatter Plot** of attendance vs exam score  
- 📌 **Box Plot** of performance vs motivational factors  
- 📌 **Violin & Bar Plots** for categorical feature impacts  
- 📌 **Count Plot** for performance-level distribution  

---

## ✅ Tools & Libraries

- **Python 3.10+**
- **Pandas**, **NumPy**
- **Seaborn**, **Matplotlib**, **Plotly Express**

---

## 🚀 Results & Outcome

- Identified top and at-risk students using performance segmentation  
- Revealed strong positive correlation between study hours, tutoring, and exam scores  
- Showed that low attendance and low motivation significantly correlate with poor performance  
- Created actionable dashboards for educators

---

## 📈 Future Improvements

- Integrate time-series performance tracking  
- Add predictive models for dropout probability  
- Deploy dashboard with Streamlit or Dash for real-time insights  

---

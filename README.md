# Student Mental Health K-Means Clustering Analysis

**Author:** Abdullahi Mohamed Jibril  
**Course:** Applied Machine Learning for Analytics  
**Date:** August 19, 2025

## 📋 Project Overview
This project implements K-Means clustering to analyze student mental health patterns using a dataset of 101 students. The application identifies four distinct mental health profiles to support targeted intervention strategies in educational settings.

## 📊 Dataset and Methodology
The analysis uses student mental health data with 11 features including demographics, academic performance, and mental health indicators (depression, anxiety, panic attacks, treatment-seeking behavior). 

**Key preprocessing steps:**
- Handling mixed datetime formats
- Encoding categorical variables
- Standardizing features
- Optimal cluster count (4) determined using Elbow Method and Silhouette Score analysis

## 🔍 Key Findings
Four distinct student profiles were identified:

- **Cluster 0 (27 students):** High anxiety, low treatment-seeking behavior
- **Cluster 1 (22 students):** Well-adjusted with minimal mental health concerns  
- **Cluster 2 (43 students):** Depression present but actively seeking help
- **Cluster 3 (9 students):** At-risk with panic attacks but no treatment engagement

## ⚡ Challenges Overcome
- Successfully resolved mixed datetime format parsing
- Implemented proper categorical encoding
- Addressed missing data through median imputation
- Handled all technical challenges with robust error management and data validation

## 💡 Recommendations
1. **Immediate intervention** for Cluster 3 (at-risk students with panic attacks)
2. **Anxiety workshops** for Cluster 0 (high anxiety, low help-seeking)
3. **Enhanced support services** for Cluster 2 (depression with help-seeking)
4. **Prevention programs** for Cluster 1 (maintain wellness)

## 🔧 Technical Implementation
- **Language:** Python
- **Environment:** Google Colab
- **Libraries:** pandas, numpy, matplotlib, seaborn, scikit-learn
- **Algorithm:** K-Means clustering with k=4
- **Testing:** Comprehensive unit testing (100% pass rate)
- **Quality:** Clean, well-commented code with effective data visualization

## 📈 Impact and Value
This clustering analysis provides educational institutions with actionable insights for:
- Resource allocation
- Targeted mental health interventions
- Early identification of at-risk students
- Personalized support strategies to improve student wellbeing and academic outcomes

## 🚀 Usage
```python
# Load and preprocess data
df = pd.read_csv('Student Mental health.csv')
# Apply clustering
kmeans = KMeans(n_clusters=4, init='k-means++', random_state=42)
clusters = kmeans.fit_predict(X_scaled)
```

## 📁 Files
- `student_mental_health_clustering.py` - Main application code
- `Student Mental health.csv` - Original dataset
- `student_mental_health_clustered.csv` - Results with cluster assignments
- `README.md` - This file

## 📝 License
This project is for educational purposes as part of Applied Machine Learning for Analytics coursework at Nexford Universtiy. 

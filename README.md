# Clinical Data Visualisation: Spotify Audio Feature Analysis
### MSc Data Science | Module: INF4000 | Grade: 83%

## 🎯 Research Objective
To investigate how key audio features (danceability, energy, loudness, and tempo) vary across categories of **Valence (Mood)** within the Spotify Tracks Dataset (114,000 records). 

The project focus was not merely on the data, but on the application of the **ASSERT framework** to engineer visualisations that manage cognitive load and remain accessible to all users.

---

## 🛠️ Methodology & Frameworks
* **ASSERT Model:** Systematically applied to guide the transition from raw data to communicative insight.
* **Grammar of Graphics:** Implemented via `ggplot2` in **R** to create a multi-layered composite visualisation.
* **Data Transformation:** Categorised continuous valence variables into Negative, Neutral, and Positive levels to enable comparative analysis.

## ♿ Inclusive Design & Clinical Perspective
Drawing on **17 years of diagnostic intuition in optometry**, I implemented high-stakes visual standards to prevent "diagnostic error" in data interpretation:
* **CVD Optimisation:** Utilised the `viridis` palette to ensure visualisations are accessible to users with **Colour Vision Deficiency**.
* **Cognitive Load Management:** Optimized the **data-ink ratio** to enhance the signal-to-noise ratio, a principle vital for diagnostic accuracy.
* **Legibility Standards:** Standardised typography and faceted layouts to support inclusive and reliable data storytelling.

---

## 📈 Composite Visualisation Components
1. **Violin & Boxplots:** Distribution of *Danceability* across Valence categories.
2. **Correlation Matrix:** Identifying relationships between features such as *Energy* and *Loudness*.
3. **Density Plots:** Comparison of feature distributions by mood category.
4. **Grouped Bar Charts:** Analysis of variance across key audio attributes.



## 📝 Key Findings
* Higher valence (positive mood) correlates with increased **danceability** and more consistent **energy** levels.
* Insights suggest that mood-based categorisation can significantly enhance the precision of personalised recommendation algorithms.

---
## 📁 Repository Structure
* `/code`: R scripts for data processing and `ggplot2` implementation.
* `/visualisations`: Final high-resolution composite plot.
* `/report`: Detailed reflection on design choices and the ASSERT framework application.

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
* **CVD Optimisation:** Utilised colour-blind safe palettes to ensure visualisations are accessible to users with **Colour Vision Deficiency**.
* **Cognitive Load Management:** Optimised the **data-ink ratio** to enhance the signal-to-noise ratio, a principle vital for diagnostic accuracy.
* **Legibility Standards:** Standardised typography and faceted layouts to support inclusive and reliable data storytelling.

---

## 📈 Composite Visualisation Components
1. **Violin & Boxplots:** Distribution of *Danceability* across Valence categories.
2. **Correlation Matrix:** Identifying relationships between features such as *Energy* and *Loudness*.
3. **Density Plots:** Comparison of feature distributions by mood category.
4. **Grouped Bar Charts:** Analysis of variance across key audio attributes.

---

## 📁 Repository Structure
* **`code/inf4000-spotify-analysis.R`**: R script for data processing and `ggplot2` implementation. Configured with a remote URL for full reproducibility.
* **`data/inf4000-spotify-tracks.csv`**: The complete Spotify Tracks Dataset (114,000 records) utilised for the primary analysis.
* **`visualisations/inf4000-valence-analysis-composite.png`**: Final high-resolution composite plot.
* **`report/inf4000-data-visualisation.pdf`**: Detailed reflection on design choices and the ASSERT framework application.

---

## 🚀 How to Reproduce
The analysis script is designed for autonomy. 
1. Clone this repository.
2. Open the script in `/code` and run. It will pull the source data directly from this GitHub repository to ensure consistent results.

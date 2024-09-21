# Entry-Level Luxury Car Brand Analysis 🚗

## 📋 Project Overview

This project analyzes **consumer conversations** from **Edmunds forums** to gain insights into the **entry-level luxury car market**. By analyzing the frequency and context of brand mentions, we provide strategic insights into **consumer perceptions**, **aspirational brands**, and **competitor positioning**. The analysis includes **co-occurrence matrices**, **lift calculations**, and **Multi-Dimensional Scaling (MDS)** for visualizing brand relationships.

### 🔍 Key Objectives:
- Identify **aspirational brands** based on consumer discussions.
- Understand **brand comparisons** through co-occurrence analysis.
- **Calculate lift ratios** to highlight brand associations.
- Provide **business insights** on brand positioning and competition.

---

## 💼 Business Problem

**JD Power & Associates** aims to perform a **competitive analysis** of the **entry-level luxury car market** using social media discussions. This analysis answers questions such as:
- **Which brand is the most aspirational?**
- **How do consumers compare brands?**
- **What are the strongest brand associations?**

---

## 📊 Analysis Pipeline

### 1. **Data Collection**
   - Data scraped from the **Edmunds Entry-Level Luxury Performance Sedans** [forum](https://forums.edmunds.com/discussion/2864/general/x/entry-level-luxury-performance-sedans).
   - Over **5000+ posts** with mentions of **various car brands** and consumer aspirations.

### 2. **Data Preprocessing**
   - Cleaning posts: Removing noise, punctuation, and converting car models into their respective brands.
   - Identifying **aspirational phrases** such as "want to," "dream of," and "aspire to."

### 3. **Co-occurrence Matrix**
   - Captures how frequently two brands are mentioned together in the same discussion.
   - Highlights which brands are compared most often by consumers.

### 4. **Lift Ratio Calculations**
   - **Lift ratios** show the strength of association between brands, indicating if two brands are mentioned together more than expected by chance.
   - Example: **Volkswagen and Audi** have the highest lift ratio, reflecting their shared ownership.

### 5. **Multi-Dimensional Scaling (MDS)**
   - Visualization using MDS to map how **brands are positioned** relative to one another based on lift ratios.
   - Example: **Mercedes** and **Subaru** are outliers, reflecting their **niche positions**.

---

## 📈 Key Analysis Results

- **Co-occurrence Matrix**:
  - **BMW** and **Acura** are frequently compared, indicating strong competition.
  - **Toyota** and **Honda** are often mentioned together, especially around discussions of **affordability** and **reliability**.
 ![image](https://github.com/user-attachments/assets/305418a5-bae9-4f49-ac72-4bebb05397d3)


- **Lift Ratios**:
  - **Volkswagen and Audi** have the highest lift value (**3.2069**), showing strong brand association.
  - **Toyota and Honda** have a lift value of **3.0502**, highlighting frequent comparisons in the **affordable car market**.
![image](https://github.com/user-attachments/assets/b079edb5-c894-4405-9be9-32edba7cdbf4)

- **MDS Plot**:
  - **Audi, BMW, Lexus, Infiniti**, and **Acura** cluster closely, indicating frequent consumer comparisons in the **luxury market**.
  - **Mercedes** and **Subaru** are far from other brands, reflecting their **distinct market positions**.
![image](https://github.com/user-attachments/assets/7b377e8a-7615-4f35-82f1-e5af02121489)

---

## 📊 Business Insights

### 🔝 **Toyota as the Most Aspirational Brand**
- **Insight**: Toyota frequently appears in discussions with **aspirational phrases**, driven by its reputation for **reliability** and **hybrid technology**.
- **Recommendation**: Toyota should highlight its leadership in **green technologies** and **sustainability**, emphasizing its hybrid models.

### 🏎️ **BMW vs. Acura - Strong Comparisons**
- **Insight**: BMW and Acura are heavily compared, particularly in the **entry-level luxury market**.
- **Recommendation**: BMW should emphasize its **performance and driving experience**, while Acura can market itself as a more **affordable luxury alternative**.

### 🚗 **Volkswagen and Audi - Cross-Brand Marketing**
- **Insight**: Volkswagen and Audi are often mentioned together, reflecting strong associations due to **shared ownership**.
- **Recommendation**: Cross-brand marketing campaigns should highlight **Volkswagen’s affordability** alongside **Audi’s premium features**.

### 🌄 **Subaru's Niche Positioning**
- **Insight**: Subaru is infrequently compared to other brands, reflecting its niche appeal as an **adventure and rugged vehicle** brand.
- **Recommendation**: Subaru should continue targeting **outdoor enthusiasts** and focus on its **all-wheel-drive models**.

---

## 📂 Project Structure

```

├── data/
│   ├── edmunds_forum_posts.csv  # Forum posts data
│   ├── car_models_and_brands_v1.csv  # Model-to-brand mapping
├── notebooks/
│   ├── Luxury Car Consumer Perception Analysis.ipynb  # Python notebook
├── README.md  # Project overview and instructions
```

## 🔮 Conclusion

This project provides valuable insights into the **entry-level luxury car market**, helping brands like **Toyota, BMW, Audi**, and **Acura** better understand their **market positioning**, **consumer comparisons**, and **aspirational appeal**. These insights can inform **marketing strategies**, **brand differentiation**, and **customer engagement** to maximize brand loyalty and appeal.

---

## 🛠️ Tech Stack

- **Python**
- **Pandas** for data manipulation
- **Matplotlib** for visualizations
- **scikit-learn** for MDS plotting
- **BeautifulSoup** for web scraping

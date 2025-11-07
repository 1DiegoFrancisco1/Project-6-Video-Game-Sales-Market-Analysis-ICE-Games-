# 🎮 Project 6 — Video Game Sales & Market Analysis (ICE Games)

### 🏢 Project Context
You work as a data analyst for the global online video game retailer **ICE**.  
Your mission is to identify patterns that determine whether a game is likely to succeed.  

By analyzing **historical sales**, **user and critic reviews**, **genres**, **platforms**, and **ESRB ratings**,  
you’ll help the company **forecast demand for 2017** and plan **targeted marketing campaigns**.  

Although the dataset covers data up to **2016**, the analytical logic can be applied to any future market forecast.

---

## 📂 Dataset Overview
Each row represents a video game title with attributes such as:

| Column | Description |
|---------|--------------|
| `name` | Game title |
| `platform` | Gaming platform (e.g., PS4, Xbox One, PC) |
| `year_of_release` | Release year |
| `genre` | Game genre |
| `na_sales`, `eu_sales`, `jp_sales`, `other_sales` | Regional sales (in millions of copies) |
| `critic_score`, `user_score` | Expert and player ratings |
| `rating` | ESRB category (E, T, M, etc.) |
| `publisher` | Game publisher |

---

## 🧹 Step 1 — Data Cleaning & Preparation
We started by **renaming columns**, **imputing missing values**, and **converting data types** to ensure consistency.  
After removing invalid entries, we focused on the **most recent five years** to capture the **active console generation**.

🎯 **Active platforms (as of 2016):**  
**PS4**, **Xbox One (XOne)**, **3DS**, **Wii U**, and **PSV**.

This gave us a clean dataset ready for analysis and trend forecasting.

---

## 📈 Step 2 — Platform Analysis

We identified the **top-selling platforms** and their evolution over time:

| Ranking | Platform | Trend |
|----------|-----------|--------|
| 🥇 | **PS4** | Rapid growth — dominant global platform |
| 🥈 | **PS3** | Declining, previous generation |
| 🥉 | **X360** | Near plateau |
| 4️⃣ | **3DS** | Stable, strong in Japan |
| 5️⃣ | **XOne** | Moderate growth, strong in USA |

- The **average life cycle** between new console generations was **≈7.6 years**.  
- **Investment recommendation for 2017:** prioritize **PS4** and **XOne** titles.

---

## 🕹️ Step 3 — Genre Trends

We analyzed the global sales by genre and found:

| Genre | Total Sales (M) | Avg Sales per Game (M) |
|--------|------------------|-------------------------|
| **Action** | 440 | — |
| **Shooter** | 305 | 1.29 |
| **RPG** | — | — |
| **Sports** | — | 0.67 |
| **Adventure / Strategy / Puzzle** | Low sales overall | — |

🎯 **Key findings:**
- *Action* and *Shooter* dominate global sales.  
- *Shooter* and *Sports* are the **most profitable genres per title**.  
- *Adventure*, *Strategy*, and *Puzzle* games sell much less but require **smaller budgets**.

💡 **2017 Marketing Insight:**
- In **North America (NA)** and **Europe (EU)** → prioritize *Shooter* and *Action* for **PS4/XOne**.  
- In **Japan (JP)** → focus on *JRPG*, *Platformers*, and *Miscellaneous* genres — smaller budgets but steady demand.

---

## ⭐ Step 4 — Ratings & Review Impact

We studied the correlation between **sales and reviews**:

- **Critic scores** showed a **clear positive relationship** with sales.  
- **User scores** had **high variance**, affecting long-term sales more than launch sales.  
- **ESRB ratings** strongly influenced regional performance:
  - **M (Mature)** titles sold best in **NA** and **EU**.
  - **E (Everyone)** and **T (Teen)** titles dominated **Japan**.

🎯 **Recommendation:**  
- Secure strong **critic reviews** for “day-one” impact.  
- Use **user feedback** later to drive **post-launch content (DLCs, expansions)**.

---

## 📊 Step 5 — Hypothesis Testing

### 🔹 Hypothesis 1 — Platform Ratings
**H₀:** The average user score for Xbox One equals that of PC.  
**H₁:** The means differ.

✅ Result: The null hypothesis was **rejected** → *PC games tend to have higher user scores*.

---

### 🔹 Hypothesis 2 — Genre Ratings
**H₀:** Average user ratings for *Action* and *Sports* games are equal.  
✅ Result: Both genres have **similarly high ratings**, aligning with their **sales leadership** in the market.

---

## 🧭 Key Insights

1. **Platform Strategy:**  
   - Focus 2017 investments on **PS4 (primary)** and **XOne (secondary)** titles.  
   - Retire marketing focus on Wii U and PSV — both in decline.

2. **Genre Strategy:**  
   - Prioritize **Action/Shooter** games for Western markets.  
   - For Japan, smaller-scale **JRPGs and Platformers** remain profitable.

3. **Rating Strategy:**  
   - **M-rated** games dominate Western regions.  
   - Optimize ESRB targeting for each region’s preferences.

4. **Review Strategy:**  
   - Push **critic engagement pre-launch**.  
   - Encourage **user engagement post-launch** to sustain revenue via updates/DLCs.

---

## 🧠 Conclusion

We identified clear **platform, genre, and regional patterns** shaping game success.  
Sales performance depends heavily on **console generation**, **genre selection**, and **ESRB targeting**.  
By aligning **game releases and marketing campaigns** with these insights, ICE can maximize ROI in 2017 and beyond.

---

## 🧰 Tools and Libraries
- **Python**, **Pandas**, **NumPy**, **Matplotlib**, **Seaborn**, **SciPy**
- Jupyter Notebook for EDA and statistical testing
- Visualization techniques: boxplots, histograms, and correlation heatmaps

---

## 🧾 Deliverables
- Cleaned and prepared dataset for analysis.  
- Exploratory data analysis of platforms, genres, and ratings.  
- Hypothesis testing on platform and genre comparisons.  
- Strategic recommendations for 2017 campaign planning.

---

## 👨‍💻 Author
**Diego Francisco Domínguez Aguilar**  
_Data Science Bootcamp – TripleTen (2025)_  

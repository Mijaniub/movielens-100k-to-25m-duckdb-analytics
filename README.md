# MovieLens Scale Analysis: 100K → 25M with DuckDB

This project explores how analytical insights evolve as we scale from the **MovieLens 100K** dataset to the **MovieLens 25M** dataset. Using **DuckDB** and **Python**, we analyze user ratings, genre trends, popularity patterns, and statistical stability across different dataset sizes.

---

## 📌 Project Overview

The main objective of this project is to understand:

- How movie rating patterns change as data volume grows  
- Whether genre trends stay consistent between small and large datasets  
- How popularity correlates with average movie ratings  
- How DuckDB performs on analytical workflows at different scales  

We first prototype our logic using the smaller **100K dataset**, then seamlessly scale the same workflow to **25M records**.

---

## 🛠️ Tech Stack

- **DuckDB** — columnar in-process analytical database  
- **Python** — data processing and analysis  
- **Pandas** — data manipulation  
- **Jupyter Notebook** — interactive exploration  

---

## 📊 Datasets

### **MovieLens 100K**
- 100,000 ratings  
- 943 users  
- 1,682 movies  
- Great for quick prototyping  

### **MovieLens 25M**
- 25,000,095 ratings  
- 162,541 users  
- 62,423 movies  
- Offers large-scale, stable statistical patterns  

Both datasets are publicly available from GroupLens.

---

## 🔍 Key Questions Explored

- Which genres dominate user ratings?
- Do top-rated movies remain the same at scale?
- How do rating distributions evolve with more data?
- Is popularity correlated with quality (average rating)?
- How stable are insights as we scale up?

---

## 📈 Highlights of Our Findings

### **1. Genre Dominance**
Drama and Comedy consistently remain the largest genres in both datasets.

### **2. Top-Rated Movies**
Classics like *The Shawshank Redemption* and *Casablanca* stay at the top even with millions of ratings.

### **3. Popularity vs Rating**
- Popular films converge around average ratings of 3.5–4.0  
- Less popular movies show more extreme ratings  
- Clear regression-to-the-mean effect at scale

### **4. User Rating Behavior**
- Few users contribute most ratings  
- Distribution remains centered around 3–4 stars  

### **5. Scaling with DuckDB**
- DuckDB handles 25M records efficiently on a single laptop  
- No distributed infrastructure needed  
- SQL logic and query structure remain unchanged when scaling  

---

## 🧠 Limitations

- MovieLens users are not representative of all movie watchers  
- Only genres and ratings were analyzed (no textual data or demographics)  
- Cloud/distributed systems are not tested here  

---

## 🚀 Future Directions

Potential improvements include:

- Adding demographic/user profiling  
- Time-series analysis of ratings  
- Cloud-based scaling (BigQuery, Athena, Snowflake)  
- Recommendation algorithms  
- Deep learning rating prediction models  

---

## 👥 Contributors

- João André Mateus Neves  
- João Leonardo Nunes Pereira  
- Gonçalo Abel Gonçalves  
- Md Mijanul Haque  

---

## 📬 Contact

If you have questions, feel free to open an issue or reach out!


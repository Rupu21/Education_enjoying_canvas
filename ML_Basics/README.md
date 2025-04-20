
# 📊 Outlier Detection from Scratch – Educational Notebook

A beginner-friendly Python notebook that explains **multiple outlier detection methods** from scratch — with code, math, and visualization. Perfect for learners, educators, and data science practitioners who want to understand the intuition *and* implementation of common techniques.

---

### 🧠 What's Inside

| Method                        | Type         | Strengths                                  |
|------------------------------|--------------|---------------------------------------------|
| Z-Score                      | Univariate   | Simple, effective for normal distributions |
| IQR (Interquartile Range)    | Univariate   | Robust against skewed data                 |
| MAD (Median Absolute Dev.)   | Univariate   | Great for heavy-tailed distributions       |
| Mahalanobis Distance         | Multivariate | Accounts for feature correlation           |
| KMeans-based Detector        | Multivariate | Unsupervised, good for clustering contexts |

---

### 🔢 Core Math Behind the Methods

- **Z-Score**:  
  \( z = \frac{x - \mu}{\sigma} \)  
  Flag if \(|z| > 3\)

- **IQR**:  
  \( \text{Outlier if } x < Q1 - 1.5 * IQR \text{ or } x > Q3 + 1.5 * IQR \)

- **MAD**:  
  \( \text{MAD} = \text{median}(|x_i - \text{median}(x)|) \)  
  Flag if \( \frac{|x - \text{median}|}{\text{MAD}} > 3.5 \)

- **Mahalanobis Distance**:  
  \( D^2 = (x - \mu)^T \Sigma^{-1} (x - \mu) \)

- **KMeans**:  
  Outliers are points farthest from their cluster centroids

---

### 📊 Visualizations Included

- Boxplot of 1D data (IQR-based outliers)
- Histogram of distribution
- 2D Scatter plot showing Mahalanobis & KMeans outliers

---

### 📦 Dependencies

```bash
pip install -r ML_Basics\requirements.txt
```

---

### 🧪 Try It Out

```python
# Run all methods on test data
z_score_outliers(data)
iqr_outliers(data)
mad_outliers(data)
mahalanobis_outliers(data_2d)
kmeans_outliers(data_2d)
```

---

### 👨‍💻 Author

Built with ❤️ by **[Your Name]**  
Contributions welcome — star, fork, and explore!

---

### 📘 License

MIT License — use freely, just give credit ✨



# 📊 Confidence Interval for Proportion – Forest Fires Dataset

This analysis estimates the proportion of **small forest fires** using a 95% confidence interval. The Parks Department uses this data to make **cost-effective decisions** on fire response resource allocation.

---

## 🔍 Objective

To determine the **confidence interval** for the proportion of forest fires considered **small**, using the `is_small` column in the dataset (values: `1` for small, `0` for not-small).

---

## ✅ Method Summary

### 1. **Calculate Sample Proportion (𝑝̂)**

Since `is_small` is binary (0 or 1), use the average:

```excel
p̂ = AVERAGE(is_small)
```

**Result:** `p̂ ≈ 0.48`

---

### 2. **Complement of p̂ (1 - 𝑝̂)**

```excel
1 - p̂ = 0.52
```

---

### 3. **Sample Size (n)**

```excel
n = COUNT(is_small)
```

---

### 4. **Set Confidence Level (95%)**

* Z-score for 95% confidence: **1.96**

---

### 5. **Calculate Margin of Error (ME)**

Formula:

```
ME = Z * √[ (p̂ * (1 - p̂)) / n ]
```

---

### 6. **Calculate Confidence Interval (CI)**

* **Lower Bound:** `p̂ - ME`
* **Upper Bound:** `p̂ + ME`

**Resulting Interval:**

```
CI = [0.4347, 0.5208]
```



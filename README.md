# Handling_Outliers_in_python

This project demonstrates how to detect and visualize **outliers in a dataset using Python**.  
The notebook calculates the **Five Number Summary** and uses the **Interquartile Range (IQR) method** to identify potential outliers. A **box plot** is also used to visualize the distribution of data.

---

## Objective

The main objective of this project is to understand how outliers can be detected in a dataset using statistical methods and visualizations.

Outliers are extreme values that differ significantly from other observations and may affect data analysis and machine learning models.

---

## Concepts Used

### 1. Five Number Summary

The **Five Number Summary** provides a quick overview of the distribution of a dataset.

It includes:

- **Minimum** – Smallest value in the dataset  
- **Q1 (First Quartile)** – 25th percentile  
- **Median (Q2)** – 50th percentile  
- **Q3 (Third Quartile)** – 75th percentile  
- **Maximum** – Largest value in the dataset  

These values help understand the spread and distribution of the data.

---

### 2. Interquartile Range (IQR)

The **Interquartile Range (IQR)** measures the spread of the middle 50% of the data.

\[
IQR = Q3 - Q1
\]

It is used to determine the boundaries for detecting outliers.

---

### 3. Outlier Detection using IQR

Outliers are identified using the following formulas:

**Lower Fence**

\[
Lower\ Fence = Q1 - 1.5 \times IQR
\]

**Upper Fence**

\[
Upper\ Fence = Q3 + 1.5 \times IQR
\]

Any value:

- Below the **Lower Fence**
- Above the **Upper Fence**

is considered a **potential outlier**.

---

## Dataset Used

A sample list of student marks is used in the notebook:

```python
lst_marks = [45, 92, 42, 47, 90, 87, 62, 13, 9, 12, 89, 96, 82, 57, 19, 1, 300, 53, 78]

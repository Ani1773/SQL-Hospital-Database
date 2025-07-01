# 🏥 SQL Project – Hospital Database Analysis

This project involves analyzing a hospital database using SQL to extract meaningful insights related to patients, doctors, treatments, billing, and department efficiency. It demonstrates my proficiency in writing complex SQL queries, data modeling, and healthcare-related data analysis.

---

## 📘 Project Description

I analyzed a simulated hospital database containing information about patients, doctors, treatments, billing, appointments, and departments. The goal was to extract meaningful patterns and generate key metrics that support hospital administration and operations.

---

## 🧠 Objectives

- Analyze patient distribution across departments
- Track doctor performance and patient load
- Evaluate hospital revenue and billing trends
- Derive insights into treatment frequency and efficiency
- Practice advanced SQL operations on realistic healthcare data

---

## 🛠 Tools & Technologies

- **Database**: MySQL 
- **Techniques**:  
  - Joins (INNER, LEFT, RIGHT)  
  - Aggregate Functions (COUNT, SUM, AVG)  
  - Subqueries & CTEs  
  - Window Functions  
  - Grouping & Filtering  

---


---

## 🔍 Sample Insights

- Total number of patients by department
- Most visited department and busiest doctor
- Monthly hospital revenue and average treatment cost
- Patients with the highest bills
- Appointments per doctor and day

---

## 🧾 Sample Query Snippet

```sql
-- Top 5 departments by patient volume
SELECT d.department_name, COUNT(p.patient_id) AS total_patients
FROM patients p
JOIN departments d ON p.department_id = d.department_id
GROUP BY d.department_name
ORDER BY total_patients DESC
LIMIT 5;




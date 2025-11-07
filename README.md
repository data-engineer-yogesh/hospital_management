# Hospital Management

Let’s complete the final dataset: the Hospital Management System, one of the most commonly asked domains in SQL  it naturally covers joins, aggregations, date logic, and subqueries.
We’ll structure this exactly like the previous datasets (Easy → Medium → Hard) using your defined learning patterns.

Assumed schema:
* patients(patient_id, name, gender, age, city)
* doctors(doctor_id, name, specialty, experience_years)
* appointments(appointment_id, patient_id, doctor_id, appointment_date, diagnosis, fees)
* treatments(treatment_id, appointment_id, treatment_type, cost, treatment_date)
* medications(med_id, treatment_id, medicine_name, dosage, duration_days)

----

SQL Practice Set — Hospital Management Dataset (30 Questions)

Level 1: Easy (Basics, Filtering, Aggregation)
Focus: SELECT, WHERE, ORDER BY, basic aggregates.

1. List all patients with their city and age.
2. Find all doctors who have more than 10 years of experience.
3. Display all appointments made after '2024-01-01'.
4. Count how many total patients are registered.
5. Find the total number of appointments per doctor.
6. Show all treatments that cost more than ₹5,000.
7. Display all medicines prescribed with a duration over 10 days.
8. Retrieve patients who live in 'Mumbai'.
9. Find the average treatment cost across all appointments.
10. List all unique specialties available in the hospital.
  - Concepts used: SELECT, WHERE, COUNT, SUM, AVG, DISTINCT, ORDER BY.

----

Level 2: Medium (Joins, Grouping, Subqueries)
Focus: multi-table joins, subqueries, grouping, HAVING.

11. List all appointments with patient and doctor names.
12. Find the total fees collected by each doctor.
13. Show the top 3 doctors who handled the most appointments.
14. Find patients who had more than 2 appointments.
15. Display doctors who treated at least one patient with “Diabetes” diagnosis.
16. Retrieve the total treatment cost per patient.
17. Find patients who have never received any treatment.
18. Show the average number of appointments handled per doctor specialty.
19. List all doctors who prescribed medicines more than 5 times.
20. Find all patients treated by doctors with more than 15 years of experience.
- Concepts used: JOIN (INNER, LEFT), GROUP BY, HAVING, Subquery, EXISTS.

----

Level 3: Hard (Analytics, CTEs, Window Functions, Business Insights)
Focus: advanced analytics, ranking, and temporal patterns.

21. Use a CTE to calculate the total treatment cost per patient, then find the top 5 patients by spending.
22. Rank doctors based on their average appointment fees (use RANK() window function).
23. Find the most common diagnosis made in the hospital.
24. Calculate the total revenue per month (using DATE_FORMAT and GROUP BY).
25. Find the average treatment cost by specialty of the doctor.
26. Identify patients who received more than average treatments.
27. Use a CTE to find the most frequently prescribed medicine.
28. For each doctor, find their first and latest appointment (using MIN and MAX).
29. Calculate the total treatment + appointment fees per patient, ordered by highest spenders.
30. Create a view doctor_performance that includes: doctor_id, total_patients_seen, avg_fees, and total_revenue.
- Concepts used:
* CTE
* Window Functions (RANK, ROW_NUMBER)
* Aggregates + JOINs
* Analytical queries (date-based, cost-based)
  
-----

##  Setup Instructions

1. **Create the database**
   ```sql
   CREATE DATABASE hospital_management_db;
   USE hospital_management_db;


## Analysis

The documentation of the data analysis process is included in the file [*hospital_management.sql*]()

## Summary

The project was done for the purpose of practice and to improve skills in SQL.

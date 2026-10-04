# Student Certification Classification using Machine Learning

## APSSDC ML Internship – Milestone Project

### Project Overview

This project classifies students as **Certified** or **Not Certified** based on their attendance across **40 training sessions**.

A student is considered eligible for certification when they attend at least **80% of the 40 sessions**.

- Total Students: 980
- Total Sessions: 40
- Minimum Attendance Required: 32 Sessions
- Certification Rule: Attendance ≥ 32 sessions → Certified
- Attendance < 32 sessions → Not Certified

The project uses **Random Forest Classification** to predict the certification status of students.

---

## Objectives

- Collect and combine attendance data from 40 sessions.
- Calculate the number of sessions attended by each student.
- Calculate attendance percentage.
- Classify students as Certified or Not Certified.
- Apply Random Forest classification.
- Visualize the certification results using graphs.

---

## Dataset

The project uses attendance data from **40 CSV files**.

Each session file contains student attendance information such as:

- Student ID
- Student Name
- Student Email
- Student Aadhaar
- Joining Time
- Leaving Time
- Session Duration
- Total Duration
- Attendance Percentage
- Attendance
- Certification Status

The 40 session files are combined and analyzed using Python.

---

## Methodology

The project follows these steps:

```text
40 Attendance CSV Files
          ↓
Combine All Sessions
          ↓
Calculate Student Attendance
          ↓
Calculate Attendance Percentage
          ↓
Certification Classification
          ↓
Random Forest Model
          ↓
Prediction and Accuracy
          ↓
Data Visualization
```

---

## Machine Learning Algorithm

### Random Forest Classifier

Random Forest is used as the machine learning algorithm.

It combines multiple decision trees to make predictions and generally provides good classification performance.

The main input feature used in the model is:

```text
Sessions Attended
```

The target variable is:

```text
Certified
```

where:

```text
1 → Certified
0 → Not Certified
```

---

## Visualizations

The project generates two graphs.

### 1. Bar Chart

The bar chart compares the number of:

- Certified students
- Not Certified students

### 2. Scatter Plot

The scatter plot represents the relationship between:

- Sessions attended
- Attendance percentage

---

## Technologies Used

- Python
- Pandas
- Matplotlib
- Scikit-learn
- Google Colab
- GitHub

---

## Python Libraries

```python
pandas
matplotlib
scikit-learn
zipfile
```

---

## Project Files

```text
Student-Certification-Classification/
│
├── student_certification.py
├── README.md
└── datasets/
    └── 40 attendance CSV files
```

---

## How to Run

### 1. Clone the repository

```bash
git clone <your-github-repository-link>
```

### 2. Open the Python file

Run:

```text
student_certification.py
```

### 3. Upload the ZIP file

The program asks for the ZIP file containing the 40 session CSV files.

### 4. Run the program

The program will:

- Extract the files
- Read all 40 sessions
- Calculate attendance
- Classify students
- Train the Random Forest model
- Display the accuracy
- Generate the bar chart
- Generate the scatter plot

---

## Certification Criteria

There are 40 sessions in total.

80% attendance is required:

```text
40 × 80 / 100 = 32 sessions
```

Therefore:

| Sessions Attended | Status |
|---|---|
| 32–40 | Certified |
| 0–31 | Not Certified |

---

## Sample Output

The program displays:

```text
Total Students         : 980
Total Sessions         : 40
Certified Students     : 725
Not Certified Students : 255
Certification Rate     : 73.98 %
Random Forest Accuracy : 100.00 %
```

The exact values may vary depending on the attendance dataset used.

---

## Future Enhancement

The project can be extended by including additional student performance factors such as:

- Assignment scores
- Quiz scores
- Participation
- Assessment marks
- Late attendance

This could make the certification prediction more comprehensive.

---

## Note on Synthetic Data

The student email IDs and Aadhaar numbers used in the dataset are **synthetically generated for educational purposes** and do not represent real individuals.

---

## Author

**APSSDC ML Internship – Milestone Project**

**Student Certification Classification using Random Forest**

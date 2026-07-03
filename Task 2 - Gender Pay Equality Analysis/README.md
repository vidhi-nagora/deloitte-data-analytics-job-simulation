# Gender Pay Equality Analysis (Excel)

## Objective

Analyze employee compensation data by classifying Equality Scores into predefined categories to identify potential gender pay inequality across different factories and job roles.

---

## Tools Used

- Microsoft Excel
- IF Function
- ABS Function

---

## Dataset

The dataset contains the following columns:

- Factory
- Job Role
- Equality Score

A new column called **Equality Class** was created based on the Equality Score.

---

## Task Performed

Created a new column named **Equality Class** to categorize each employee's Equality Score into one of three groups:

| Equality Score | Classification |
|---------------:|----------------|
| -10 to +10 | Fair |
| Less than -20 or Greater than +20 | Highly Discriminative |
| Between -20 & -10 or Between +10 & +20 | Unfair |

---

## Formula Used

```excel
=IF(ABS(C3)<=10,"Fair",IF(ABS(C3)>20,"Highly Discriminative","Unfair"))
```

---

## Formula Logic

The `ABS()` function converts both positive and negative Equality Scores into positive values before applying the conditions.

Classification logic:

- If the absolute value of the Equality Score is **10 or less**, classify it as **Fair**.
- If the absolute value is **greater than 20**, classify it as **Highly Discriminative**.
- Otherwise, classify it as **Unfair**.

Using `ABS()` ensures that both positive and negative scores are evaluated consistently.

---

## Example Classifications

| Equality Score | Equality Class |
|---------------:|----------------|
| 8 | Fair |
| -10 | Fair |
| 15 | Unfair |
| -18 | Unfair |
| 30 | Highly Discriminative |
| -45 | Highly Discriminative |

---

## Skills Demonstrated

- Data Classification
- Excel Formula Writing
- Logical Functions (IF)
- ABS Function

---

## Repository Files

- `Equality_Table_Updated.xlsx`
- `README.md`

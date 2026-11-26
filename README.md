# Customer Feedback – Text Classification & Data Annotation

## Project Overview

This project focuses on manually classifying customer feedback into predefined categories and evaluating annotation consistency through data quality checks.

The project demonstrates practical experience in data inspection, data cleaning, manual text annotation, annotation guideline development, and quality assessment using Python.

## Project Objectives

- Inspect and understand a customer feedback dataset.
- Identify duplicate records and missing values.
- Develop clear annotation guidelines.
- Manually classify customer reviews into predefined categories.
- Compare manual annotations with existing dataset labels.
- Evaluate annotation agreement using classification metrics.
- Document data quality findings and project limitations.

## Dataset Information

**Dataset:** Product Reviews Sentiment Dataset  
**Source:** Hugging Face – AnkitAI/product-reviews-sentiment  
**Original records:** 7,000  
**Unique review texts:** 320  
**Columns:** Review, Category

### Categories

1. Product Feedback
2. Customer Service
3. Fraud and Scam
4. Operational Issues

## Data Cleaning and Quality Checks

The dataset was inspected using Python and Pandas.

| Quality Check | Result |
|---|---:|
| Original records | 7,000 |
| Unique review records | 320 |
| Duplicate records removed | 6,680 |
| Missing values | 0 |
| Conflicting categories among identical reviews | 0 |

Duplicate records were removed from a separate copy of the original dataset to preserve the source data.

## Manual Annotation Process

A sample of 40 unique customer reviews was selected for manual annotation.

Each review was classified using predefined annotation guidelines. The annotation process included:

- Reading and understanding the review.
- Identifying its primary subject.
- Assigning one appropriate category.
- Recording review status.
- Adding annotation comments where applicable.

### Manual Annotation Distribution

| Category | Reviews Annotated |
|---|---:|
| Product Feedback | 25 |
| Fraud and Scam | 6 |
| Customer Service | 5 |
| Operational Issues | 4 |
| **Total** | **40** |

## Annotation Quality Assessment

Manual annotations were compared against the existing labels in the dataset.

The following evaluation metrics were calculated using Scikit-learn:

- Precision
- Recall
- F1-score
- Accuracy
- Confusion Matrix

### Results

| Category | Precision | Recall | F1-score | Support |
|---|---:|---:|---:|---:|
| Product Feedback | 1.00 | 1.00 | 1.00 | 25 |
| Customer Service | 1.00 | 1.00 | 1.00 | 5 |
| Fraud and Scam | 1.00 | 1.00 | 1.00 | 6 |
| Operational Issues | 1.00 | 1.00 | 1.00 | 4 |

**Overall agreement with existing dataset labels: 100% (40/40 reviews).**

## Tools and Technologies

- Python
- Google Colab
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn
- Google Sheets
- GitHub

## Project Structure

```text
Customer_Feedback_Data_Annotation/
│
├── dataset/
│   ├── categorized_text_reviews.csv
│   └── cleaned_unique_reviews.csv
│
├── annotations/
│   ├── manual_annotation_task.csv
│   └── annotation_quality_results.csv
│
├── notebooks/
│   └── Customer_Feedback_Data_Annotation.ipynb
│
├── reports/
│   ├── Annotation_Quality_Report.pdf
│   └── confusion_matrix.png
│
└── README.md
```

## Key Skills Demonstrated

- Data Cleaning and Preprocessing
- Duplicate Detection
- Manual Text Classification
- Data Annotation
- Annotation Guideline Development
- Data Quality Assurance
- Annotation Consistency Evaluation
- Classification Metrics
- Python Data Analysis
- Documentation and Reporting

## Project Limitations

- The original dataset contained 7,000 records but only 320 unique review texts.
- Manual annotation was performed on a sample of 40 reviews.
- Existing dataset labels were used as reference labels but were not independently verified.
- Therefore, the 100% agreement represents consistency with existing dataset labels, not independently established annotation accuracy.
- A larger sample and independent review by additional annotators would provide stronger validation.

## Conclusion

This project provided hands-on experience in customer feedback classification, manual data annotation, data quality inspection, and annotation evaluation.

The workflow demonstrates foundational skills relevant to AI data annotation, dataset preparation, text classification, and data quality assurance.
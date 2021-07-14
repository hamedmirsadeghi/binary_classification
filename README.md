Will a user become an executive?
=======================

A job marketplace  provides users with job recommendations.
One aspect of matching users and jobs is related to the career level. For example, people who are seeking
for jobs at the level of an _executive_ may feel offended in case they get internships recommended.

we would like to investigate whether we can predict whether a user will
become an executive in her next career step.


## 1. Dataset 

[dataset.csv](dataset.csv) is a tab-separated file that contains the feature vectors that can be used for designing your algorithm. 
The columns/features in the file are: 

| Feature | Description |
|:--------|:------------|
| `is_executive` | 1 if the user is in her current job an executive; otherwise: 0 |
| `career_level` | the current career level of the user. 0 = unknown, 1 = student, 2 = beginner, 3 = professional, 4 = manager, 5 = executive, 6 = senior executive |
| `discipline_id` | in what kind of discipline is the user currently working (22 disciplines; the actual meaning is not important for this task) |
| `jobrole_id` | ID of the jobrole that the user currently has |
| `industry_id` | ID of the industry (23 industries; the actual meaning is not important for this task; 0 = unknown) |
| `company_size` | an ID that describes the size of the company (0 = unknown) |
| `number_of_cv_entries` | the number of CV entries (= work experience entries) that the user lists on job poral |
| **`will_be_executive`** | the class that should be predicted: 1 = yes, the user will be at the level of an executive (i.e. `career_level >= 5`) in her next career step; otherwise: 0 |


## 2 Task 

- design a lightweight algorithm that can predict whether a user will be at the career level of an executive in her next career step and
- evaluate and discuss the quality of your algorithm

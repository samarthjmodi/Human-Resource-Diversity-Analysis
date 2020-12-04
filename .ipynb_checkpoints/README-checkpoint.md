

# Human Resource Diversity Analysis
By Samarth Modi

MS Data Science, University of Washington 

Date: Dec 15, 2020


## Abstract
With diversity and inclusion becoming crucial to the mordern workplace, it is often unclear how far we have reached today in inculcating a culture that is inclusive of personnels demonstrating diversity across race, gender, age, etc. To get a better understanding of the same, we perform an exploratory analysis of Human Resource data from an anonymous workplace. We observe that the workplace does demonstrate diversity and inclusion to a high extend, but it is far from being absolutely non-discriminatory. We learn about the differences in diversity due to recruiting sources, difference in the pay as well as about the overall diversity in the organization race, gender and age. We conclude by considering a bigger, richer dataset as well as data from multiple workplaces to extend our understanding of diversity before implying anything concrete from the current analysis.

## Introduction and Motivation

The MSDS program at UW is committed to fostering an inclusive environment for all individuals in our community by promoting diversity and inclusivity. Thus, we see that diversity and inclusion has been given a high priority at academic institutions as UW. This makes me wonder about the industrial paradigm of diversity and inclusion. By performing an exploratory analysis on Human Resource data, I wish to learn about the industrial paradigm of diversity. Specifically, I wish to have a holistic view of diversity at a typical company and have a better understanding of how far we have come with diversity and inclusion, thus bolstering our human-centered perspective of the same. This analysis will help us learn about different areas where diversity has been properly embraced, and the areas where we need to work more to include more diversity, thus making it a human centered data science project. Specifically, we would be able to check if there is either correlational or causational relationship between diversity in the workforce and certain other entities associated with the HR data of the workforce, eg. seniority, pay, gender, etc.


## Repository Structure

```
.
├── Data
|    └── HRDataset.csv
├── Figures
├── HrDiversityAnalysis.ipynb
└── LICENSE
```


- [Data](https://github.com/samarthjmodi/data-512-final/tree/main/Data): Directory containing the dataset used.
- [HrDiversityAnalysis.ipynb](https://github.com/samarthjmodi/data-512-final/blob/main/Data/HRDataset.csv): The dataset used in this analysis.
- [Figures](https://github.com/samarthjmodi/data-512-final/tree/main/Figures): Directory containing all of the figures generated during the analysis in the Jupyter notebook.
- [HrDiversityAnalysis.ipynb](https://github.com/samarthjmodi/data-512-final/blob/main/HRDiversityAnalysis.ipynb): Jupyter notebook that contains both my written report and my code.
- [LICENSE](https://github.com/samarthjmodi/data-512-final/blob/main/LICENSE): MIT LICENSE file for my code
- [Abstract](https://github.com/samarthjmodi/data-512-final/blob/main/Abstract.txt): A short scientific abstract of my study

## Data Source
For this analysis, I wish to use the dataset made available by Dr. Rich Huebner and Carla Patalano to accompany a case study designed for graduate HR students studying HR metrics, measurement, and analytics. The CSV revolves around an anonymous company and the core data set contains names, DOBs, age, gender, marital status, date of hire, reasons for termination, department, whether they are active or terminated, position title, pay rate, manager name, and performance score.

The dataset can be found here: [Human Resources Data Set](https://www.kaggle.com/rhuebner/human-resources-data-set) 

**Citation:** Dr. Carla Patalano, “Human Resources Data Set.” Kaggle, 2020, doi: 10.34740/KAGGLE/DSV/1572001.

The dataset has Creative Commons license, proprietary to New England College of Business, but free for use for academic purpose. Since HR data can be hard to come by, this dataset containing demographic information about the staff of this anonymous company can be deemed fit for our purpose of Diversity Analysis, and thus is very relevant to our problem statement. Since this dataset contains the names of the staff, we have an ethical responsibility to get rid of this personally identifiable information before starting our analysis and we need to make sure that any observed result cannot be mapped to any particular staff member.

## DEPENDENCIES

OS type and version: macOS Catalina, Version 10.15.7, OS build 18362.535

System type: 64-bit OS, x64-based processor

Python version: >=3.6

Python Libraries and versions:

|Python Libraries   	    |     Version            |
|---------------|:-----------------------|
|matplotlib	       |   3.3.3|
|seaborn	        |  0.11.0|
|pandas	            |1.1.4|
|numpy	            |1.19.4|

## Key Findings
 
### 1. What are our best recruiting sources if we want to ensure a diverse organization?

It's important that every organization strives to make sure their recruitment practices aren't affected by prejudices or biases.
This matter should be addressed with regards to which groups are rejected the most when searching for jobs. 
**Discrimination is an issue that constantly hits non-white people, women and elders.**

Throughout the analysis of all features, *Diversity Job Fair* proved to be vital in making this company more plural. It should only be encouraged and expanded.

Regarding race, more than half of the people hired via *Indeed* and *on-campus recruiting* are from underrepresented groups. Contrastingly, some sources need to undergo further scrutiny as to *why they only bring white employees*.

When it comes to age diversity, the organization is far behind, and no recruitment source is distinctly efficient.

### 2. Are there areas of the company where pay is not equitable?

A deep analysis has showed some wage gaps inside departments:

1. **At *IT/IS*, people of *two or more races* are paid significantly less than other workers in the same job position**. None of the data show a cause for that.

2. **Women's income is lower overall.** The gap stems mainly from two sources:
  - in *Production*, the least well-paid department, females outnumber males by some extent, which results in a greater impact in women's overall salary. Their average income is also slightly inferior in the department;
  - in *Admin Offices*, the wage gap between genders is substantial, though it is hard to tell if the distribution of functions is discriminatory.

3. **Most workers aged 50+ in *Production* work at lower-paid positions.**

### 3. What is the overall diversity profile of the organization?

**Race**

While more than half of the workforce is made of white people, we've seen before that the jobs are more well distributed along underrepresented groups comparatively to official statistics in a national level. 

*Hispanics* get a slightly higher pay rate in average, whereas *American Indian or Alaska Natives* perform lower on that variable. Considering that these groups have only four members each, it is premature to conclude the divergence is caused by any discriminatory treatment.

**Gender**

The workforce is predominantly female. Additionally, the company's CEO is a woman, and some more can be found in other high positions. These are positive, distinctive traits in a world that favors hiring male workers for most roles, especially leading ones.

A potential highlight is how the company hires many women to work in *Production*, a department where labor is often manual.

However, the company still faces some income inequality related to gender. The issue should be further investigated and dealt with.

**Age**

Only 6.4% of the workers are 55 or older. This is certainly a diversity issue, specially looking at how 2018 data from the US BLS shows that 23.1% of the workforce in the country is in that age group (https://www.bls.gov/emp/graphics/2019/labor-force-share-by-age-group.htm).

**The matter is specially precarious in the Software Engineering department and Admin Offices, that together count no more than a handful employees over *40*.**


*Sales*, on the other hand, performs really well, having a good amount of well-paid elderly workers.

## Conclusion

By performing an exploratory analysis on the Human Resource data, we learned about the industrial paradigm of diversity. We tried to have a holistic view of diversity at a typical company and have a better understanding of how far we have come with diversity and inclusion, thus bolstering our human-centered perspective of the same. However, as mentioned in the previous section, we successfully understand the diversity paradigm of the anonymous company, but fail to extend the findings to the workforce population. This analysis will helped us learn about different areas where diversity has been properly embraced at the anonymous company, and the areas where we need to work more to include more diversity, thus making it a human centered data science project.

We learn that Diversity Job Fair proved to be vital in making this company more plural. It should only be encouraged and expanded. We also learn that Women and workers aged 50+ in Production work belong to the lesser paid strata of the company. We assessed the diversity of the company with respect to race, gender and age, and a good amout of learning from the same. Overall, we can say that the anonymous company is a generally diverse company, though it still has some faults. The biggest issue is the lack of age diversity, which is not truly promoted by any recruitment source. The organization should review its hiring practices to remove any potential bias. Further research is required to extend the analysis to a larger audience and improve its generalizability. But overall, we can safely say that the society has progressed towards more diversity, and it has become more inclusive, though there is still scope of improvement.


---
# Do not edit the text between these lines!
layout: default
---

# Navigating the On-Ramp: Analyzing Prior Experience in COMP110

<img src="./static/imgs/logo.png" alt="COMP110 Logo" width="500"/>

## Project Overview: Continuous Improvement
In this project, I explored how prior programming experience impacts a student's journey through COMP110. Using a dataset of anonymized survey responses from current students, I aimed to identify if "true beginners" (those with less than one month of experience) face disproportionate hurdles in understanding and difficulty. 

The goal of this analysis is **Continuous Improvement**: by identifying where the "on-ramp" to computer science is steepest, the instructional staff can better tailor resources to ensure all students, regardless of background, can succeed.

---

## Data Analysis Summary
Using custom Python utility functions (including `read_csv_rows`, `columnar`, and a custom `filter_by_value` function), I processed the raw survey data to compare three key variables:
1. **Prior Experience**: The amount of programming a student did before the course.
2. **Difficulty**: A Likert scale (1-7) of how hard the student finds the course.
3. **Understanding**: A Likert scale (1-7) of how well the student feels they grasp the material.

By converting these string-based survey responses into numerical data, I was able to calculate averages and visualize the spread of student sentiment across the entire class.

---

## Visualizing the Experience Gap

### 1. The Class Profile
This chart shows the distribution of experience levels across the current semester. It highlights that a significant portion of the class enters with little to no prior exposure to coding.

<img src="./static/imgs/exp_dist.png" alt="Bar chart showing the count of students per experience level" width="600"/>

### 2. Average Understanding by Experience
As hypothesized, there is a correlation between prior experience and current understanding. Students with over a year of experience report the highest confidence, while true beginners are still finding their footing.

<img src="./static/imgs/avg_understanding.png" alt="Bar chart showing average understanding scores" width="600"/>

### 3. Difficulty Distribution
This boxplot reveals the "Difficulty" range. While some beginners find the course manageable, the median difficulty for those with no experience is notably higher than for those with a high school coding background.

<img src="./static/imgs/difficulty_box.png" alt="Boxplot showing the distribution of difficulty ratings" width="600"/>

---

## Final Conclusions and Recommendations

My analysis confirms that while COMP110 is designed as an introductory course, the "experience gap" significantly impacts perceived difficulty and student confidence. 

### Key Findings:
* **True Beginners** report a median difficulty score of 5/7, compared to 3/7 for experienced students.
* **Understanding** scores remain relatively high across all groups, suggesting that while the course is hard, the teaching methods are effective.

### Recommendations for Improvement:
To create more value for the "Beginner" stakeholder group, I recommend implementing **"Syntax-First" workshops** in the first three weeks of the semester. This would help bridge the gap for students who have never seen a `for` loop or a `variable` before, allowing them to focus on logic rather than just notation.

**Potential Trade-offs:** Redirecting TA resources to beginner-only sessions may decrease the availability for advanced students, but it ensures a more equitable learning environment for the majority of the enrollment.

---

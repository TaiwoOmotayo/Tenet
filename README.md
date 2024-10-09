# Tenet
Datafest project on leveraging data analytics to enhance student performance in African secondary schools, focusing on JAMB and WASSCE exams.

# Student Performance Enhancement Project

**Description**:  
This project aims to address the problem of a large number of African students, specifically Nigerian secondary school students, scoring below average in national examinations such as WAEC, JAMB, and final secondary school exams. The goal is to build a data-driven solution that helps these students improve their scores and achieve above-average performance.

---

## Table of Contents

1. [Introduction](#introduction)
2. [Problem Statement](#problem-statement)
3. [Project Structure](#project-structure)
4. [Data Overview](#data-overview)
5. [Usage](#usage)
6. [Deployment](#deployment)
7. [Recommendations](#recommendations)
8. [License](#license)
9. [Contact](#contact)

---

## Introduction

The project's primary focus is on improving the performance of Nigerian secondary school students in their final examinations. We generated and analyzed data reflecting the Nigerian secondary school system, student demographics, and academic performance. Through strategic data collection and machine learning models, we built a system to predict and enhance student outcomes.

---

## Problem Statement

A significant number of African students score below average in important exams such as WAEC, JAMB, and their final school assessments. The project's goal is to create a system that uses generated data and machine learning models to predict student performance and offer targeted interventions to help students score above average.

---

## Project Structure

The project consists of multiple teams working together:
- **Data Engineers**: Designed and implemented a data warehouse using SQL Server for easy data access.
- **Data Analysts & Data Scientists**: Analyzed the data and developed machine learning models to predict student performance.
- **Deployment Team**: Developed a web-based solution for model deployment.

---

## Data Overview

We generated seven tables to reflect different aspects of the Nigerian secondary school system and student details. While some data were collected directly from students and their parents, others were gathered through strategic questionnaires and assessments.

**Generated Tables and Columns**:

1. **teacher**  
   - teacher_id  
   - gender  
   - qualifications  
   - salary  

2. **study_habits**  
   - student_habit_id  
   - student_id  
   - study_location  
   - conducive_learning_environment  
   - study_preference  
   - internet_usage_for_study  

3. **student_attendance**  
   - student_Attendence_id  
   - student_id  
   - term  
   - class  
   - total_days  
   - reasons  
   - days_present  

4. **student**  
   - student_id  
   - date_of_birth  
   - gender  
   - department  
   - class  
   - number_of_siblings  
   - interest_in_further_education  
   - extra_lesson  
   - academic_year  
   - status  
   - parent_id  
   - educational_habit_id  

5. **parents**  
   - parent_id  
   - student_id  
   - parent_educational_level  
   - household_income  
   - parents_employment_status  
   - parental_support_at_home  
   - parent_school_interaction  

6. **exam_performance**  
   - exam_performance_id  
   - student_id  
   - academic_year  
   - subject  
   - exam_type  
   - term  
   - grade  
   - score  
   - class  
   - teacher_id  
   - parent_id  

7. **educational_habit**  
   - educational_habit_id  
   - student_id  
   - complete_curriculum  
   - learning_rate  
   - exam_writing_manner  
   - referencing  
   - recommended_textbook_usage  
   - rivalry_competition  
   - motivation_type  
   - self_confidence  
   - commitment_to_education  

---

## Usage

To train or use the machine learning models:
- Open the `DATATHON student performance prediction.ipynb` file and run the Jupyter Notebook to see the code for machine learning models.
- Use the provided `Jamb_prediction.sav` model for JAMB score predictions.
- Use the `Final_exam.sav` model for O-level subject grade predictions.

---

## Deployment

To deploy the project, use the provided `index.html` and `deploy.py` files:
1. `index.html`: The web interface for user interaction.
2. `deploy.py`: Handles the backend logic for deploying the machine learning models.

---

## Recommendations

### Key Recommendations to stakeholders to help students get above average (Combination of A1's, B2's, and B3's):

1. **Attendance Monitoring (5.73%)**:
   - **Absenteeism Strategies**: Implement tracking systems to monitor attendance closely. Create incentives for good attendance and engage with families to understand reasons for absences.

2. **Study Location (5.30%)**:
   - **Optimal Study Environments**: Educate students and parents on creating conducive study environments at home. Provide resources for improving study locations, like quiet spaces with adequate lighting.

3. **Teacher Qualification (4.60%)**:
   - **Professional Development for Teachers**: Invest in continuous training for teachers to enhance their teaching methods and subject knowledge, ensuring they are well-equipped to support students.

4. **Motivation Type (4.40%)**:
   - **Personalized Motivation Programs**: Identify what motivates each student and tailor motivation strategies accordingly, such as rewards for academic achievements or recognition programs.

5. **Parental Educational Level (4.22%)**:
   - **Parent Education Programs**: Offer workshops for parents to improve their understanding of the educational system and how they can support their children's academic success.

6. **Household Income (3.96%)**:
   - **Financial Aid Awareness**: Provide information on scholarships and financial aid options to ensure students from low-income families can access resources they need for success.

7. **Study Preference (3.87%)**:
   - **Individualized Learning Plans**: Develop study plans tailored to each student’s learning preferences, integrating diverse study methods such as group work, independent study, and online resources.

8. **Exam Writing Skills (3.84%)**:
   - **Exam Preparation Workshops**: Conduct sessions focused on improving exam writing skills, including time management, answering techniques, and stress management.

9. **Learning Rate (3.43%)**:
   - **Adaptive Learning Technologies**: Use technology to provide adaptive learning experiences that cater to the pace at which each student learns.

10. **Gender Considerations (2.86%)**:
    - **Gender-Sensitive Approaches**: Develop strategies that address any potential biases or challenges based on gender, ensuring equal support for all students.

11. **Recommended Textbook Usage (2.49%)**:
    - **Textbook Accessibility**: Ensure that all students have access to recommended textbooks, possibly through library systems or digital resources.

12. **Conducive Learning Environment (2.47%)**:
    - **School Environment Enhancements**: Focus on creating a supportive and encouraging school atmosphere, including safe spaces for learning and social interactions.


Stakeholders should implement a **data-driven approach** by continuously monitoring these factors and their impact on student performance. Regularly collect feedback from students, parents, and teachers to refine the strategies and ensure they are effectively promoting higher grades.


---

### Recommendations Based on Correlation and Feature Importances to have above average in JAMB

1. **Focus on Learning Rate (20.16%)**:
   - **Personalized Learning Approaches**: Implement strategies that cater to individual learning speeds. Regular assessments can help tailor learning plans that enhance students' grasp of materials.

2. **Enhance Parental Support at Home (13.77%)**:
   - **Parent Training Programs**: Conduct workshops to equip parents with strategies to create a supportive learning environment, encouraging consistent study habits at home.

3. **Increase Parent-School Interaction (11.30%)**:
   - **Structured Communication Channels**: Establish regular meetings or platforms (like newsletters) for parents and teachers to discuss student progress, ensuring parents are engaged and informed.

4. **Utilize Recommended Textbook Usage (10.87%)**:
   - **Diverse Learning Resources**: Encourage the use of recommended textbooks alongside supplementary materials (online resources, videos) to enhance understanding and retention.

5. **Foster Commitment to Education (9.30%)**:
   - **Goal Setting Initiatives**: Encourage students to set educational goals and monitor their progress, cultivating a sense of ownership and commitment to their studies.

6. **Implement Extra Lessons (4.59%)**:
   - **After-School Tutoring Programs**: Provide additional support through after-school programs to reinforce difficult concepts and boost academic performance.

7. **Cultivate Interest in Further Education (3.93%)**:
   - **Career Counseling Sessions**: Introduce students to various career paths and the educational requirements, helping them understand the value of academic achievement for their future.

8. **Build Self-Confidence (3.81%)**:
   - **Recognition Programs**: Create a system for acknowledging student achievements, fostering a positive self-image and motivation to excel.

9. **Complete Curriculum Engagement (3.41%)**:
   - **Tracking System for Curriculum Completion**: Monitor students’ progress through the curriculum, offering support to those falling behind to ensure all components are covered.

10. **Encourage Active Parental Involvement in Education (2.91%)**:
    - **Family Involvement in Learning Activities**: Encourage families to participate in educational activities or events, strengthening the link between home and school.

11. **Understand the Influence of Student Age (4.95%)**:
    - **Age-Appropriate Teaching Methods**: Tailor teaching strategies to align with developmental stages, ensuring the material is relatable and engaging.

12. **Assess the Impact of Study Preferences (0.96%)**:
    - **Learning Style Assessments**: Help students identify their preferred study methods and provide resources that align with these styles to enhance engagement and effectiveness.

13. **Facilitate a Conducive Learning Environment (0.69%)**:
    - **Classroom Environment Enhancements**: Create an environment that minimizes distractions and promotes focus, incorporating flexible seating arrangements and quiet study areas.


---


## Contact of Contributors

- **Data Engineer**: your-name
- **Email**: m
- **LinkedIn**: []([])
- **Twitter(X)**: []([])
- **Portfolio**: []([])
- 
- - **Data Analyst**: your-name
- **Email**: taiwo.s.omotayo@gmail.com
- **LinkedIn**: []([])
- **Twitter(X)**: []([])
- **Portfolio**: [Taiwo Omotayo]([])
- 
- - **Data Scientist**: Taiwo Omotayo
- **Email**: taiwo.s.omotayo@gmail.com
- **LinkedIn**: [Taiwo Omotayo]([https://www.linkedin.com/in/taiwo-omotayo])
- **Twitter(X)**: [Taiwo Omotayo]([https://www.x.com/omotayotaiwo18])
- **Portfolio**: [Taiwo Omotayo]([https://linktr.ee/TaiwoOmotayo])
  


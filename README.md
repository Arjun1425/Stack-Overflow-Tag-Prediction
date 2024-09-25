# Stack-Overflow-Tag-Prediction

![image](https://github.com/user-attachments/assets/5e09908b-fa3a-474b-b638-816e4d602a0e)

This repository contains the implementation of a machine learning model for **Tag Prediction** on Stack Overflow questions. The goal is to suggest relevant tags based on the content of the questions posted on the platform, helping users to categorize their questions effectively.

## 1. Business Problem

### 1.1 Description

**Stack Overflow** is the largest and most trusted online community for developers to learn, share knowledge, and build their careers. It features questions and answers on a wide range of programming topics. Each month, over 50 million developers visit the platform to find solutions to their programming challenges.

Tags play a crucial role on Stack Overflow, as they help categorize questions and make them more accessible to others with relevant expertise. However, it can be difficult for users to always select the appropriate tags. This project aims to build a model that can predict the relevant tags based on the content of the questions.

### Problem Statement

The task is to predict the tags associated with a question based on its content. These tags help in organizing and categorizing the questions, making it easier for users to find and answer them.

- **Source**: [Kaggle Competition](https://www.kaggle.com/c/facebook-recruiting-iii-keyword-extraction/)

## 1.2 Source / Useful Links

- **Data Source**: [Kaggle Competition Dataset](https://www.kaggle.com/c/facebook-recruiting-iii-keyword-extraction/data)
- **Youtube Video**: [Video on Tag Prediction](https://youtu.be/nNDqbUhtIRg)
- **Research Paper 1**: [Tagging and Keyword Extraction](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/02/tagging-1.pdf)
- **Research Paper 2**: [Paper on Tagging Techniques](https://dl.acm.org/citation.cfm?id=2660970&dl=ACM&coll=DL)

## 1.3 Real World / Business Objectives and Constraints

- **Objective**: Predict as many relevant tags as possible for a given question with high precision and recall.
- **Constraints**:
  - Incorrect tag predictions can negatively impact user experience on Stack Overflow.
  - There are **no strict latency constraints**, meaning that the prediction does not need to be in real-time.
  - Achieving a balance between **precision and recall** is crucial to ensure that relevant tags are suggested without overloading the user with incorrect ones.

## 2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## 3. Ensure that you have downloaded the dataset from Kaggle and placed it in the appropriate directory.

## 4. Data Preprocessing
  - Sample 1M data points.
  - Separate code-snippets from Body.
  - Remove Spcial characters from Question title and description (not in code).
  - Remove stop words (Except 'C').
  - Remove HTML Tags.
  - Convert all the characters into small letters.
  - Use SnowballStemmer to stem the words.

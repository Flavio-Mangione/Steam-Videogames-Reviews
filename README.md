# Repository Content

This repository contains a Jupyter notebook titled "Steam Reviews and Algorithm Analysis" The notebook is divided into two main sections:
1. **Analysis of a dataset** containing review data from the Steam gaming platform in 2021 with analysis of the results obtained in markdown structure;
2. **Algorithm complexity analysis** focused on evaluating the computational complexity of an algorithm.

# Steam Reviews 2021 Dataset

The "Steam Reviews 2021" dataset, available on [Kaggle](https://www.kaggle.com/datasets/najzeko/steam-reviews-2021), offers detailed insights into user reviews for games on the Steam platform. This dataset includes information on user ratings, gameplay time, recommendation indicators, and timestamps, making it an excellent resource for analyzing user engagement, game popularity, and sentiment trends within the gaming community.

![Top 10 Games by Sales](https://cdn.akamai.steamstatic.com/store/home/store_home_share.jpg)

## Overview

This dataset focuses on reviews posted by Steam users in 2021. Each entry provides data on user preferences, game engagement, and ratings. It is particularly valuable for researchers, data scientists, and game developers interested in exploring user behavior patterns, identifying trends in gaming popularity, and assessing sentiment.

## ⚠️ Warning 

**The following dataset is 7.6 Gigabyte in size and requires at least 24 Gigabyte of RAM for complete running of jupyter file.** If your computer does not meet these specifications, consider using a virtual machine with adequate computational power to handle the dataset efficiently.

## Key Attributes of the Dataset

- **Review details**: Data on each review, including creation and update timestamps, user recommendations, and text snippets where available.
- **User engagement**: Metrics on playtime, total review counts, and other engagement indicators.
- **Game information**: Title of the game, genre categories, and other descriptive details relevant to each game.

## Libraries

**To run the analysis in this notebook, please install the following Python libraries:**

- `kagglehub`
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `datetime`
- `scipy`
- `plotly`
- `nltk`
- `swifter`

## Data fields

The dataset consists of the following primary fields:

- **Timestamp created**: The date and time when the review was initially created.
- **Timestamp updated**: The most recent date and time when the review was updated.
- **Game title (`app_name`)**: Name of the game to which the review pertains.
- **Recommended**: Binary indicator (`True` = Recommended, `False` = Not Recommended) representing whether the user endorses the game.
- **Playtime forever**: Total playtime in minutes that the user has logged for the game at the time of the review.
- **Author details**:
  - **Last played**: Date when the reviewer last played the game.
  - **Number of reviews**: Total reviews authored by the user, indicating their engagement level on Steam.

## Potential applications

This dataset can support a range of analyses and projects, including:

- **Sentiment Analysis**: Determine general user sentiment by analyzing reviews and recommendations.
- **Engagement and Retention Studies**: Evaluate user playtime and frequency of reviews to infer engagement levels with various games.
- **Popularity and Recommendation Trends**: Assess which games received the most recommendations and explore why some games have higher review volumes.
- **Comparative analysis**: Contrast top-reviewed and top-played games to explore correlations between playtime and review volume.

## License

This dataset is sourced from Kaggle and adheres to Kaggle's usage terms. Please check Kaggle's licensing policy if considering use for commercial purposes.

# Algorithm question

![Algorithm](https://i0.wp.com/bdtechtalks.com/wp-content/uploads/2022/02/algorithm-formulation.jpg)

## Information about the Algorithm

You are given two positive integers, \( n \) (where 1 ≤ n ≤ 10^9) and k (where q ≤ k ≤ 100).Your task is to express n as the sum of k positive integers, all having the same parity (i.e., all have the same remainder when divided by 2, meaning they are either all even or all odd). In other words, find a₁, a₂, ..., aₖ, each aᵢ > 0, such that n = a₁ + a₂ + ... + aₖ, and all aᵢ simultaneously are either even or odd. If it's impossible to represent n in this way, report that no such representation exists.

### Input

In the first input line, you will receive a number t (where 1 ≤ t ≤ 100), representing the number of test cases. The following t lines will contain two values, n and k, corresponding to each test case.

### Output

For each test case, if it is possible to represent n as the sum of k positive integers, all of the same parity (either all even or all odd), print `YES` and provide the corresponding values of aᵢ in the next line. If there are multiple valid solutions, you can print any of them. If such a representation is not possible for a given test case, print `NO`.

### Examples

**Input**

```text
10 3
100 4
8 7
97 2
8 8
3 10
5 3
```

**Output**

```text
YES
4 2 4
YES
55 5 5 35
NO
NO
YES
1 1 1 1 1 1 1 1
NO
YES
3 1 1
```

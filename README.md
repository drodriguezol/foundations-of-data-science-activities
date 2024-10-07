
# Foundations of Data Science

## Menú

- [Data Organization and Structure](#data-organization-and-structure)
- [Data Sources and Types](#data-sources-and-types)
- [Data Analysis Concepts](#data-analysis-concepts)
- [How to Approach Duplicates in Data](#how-to-approach-duplicates-in-data)
- [What is Categorical Data?](#what-is-categorical-data)
- [Label Encoding Example](#label-encoding-example)
- [Python Methods Overview](#python-methods-overview)
  - [Understanding Numerical Representation](#understanding-numerical-representation)
  - [Handling Missing Data](#handling-missing-data)
  - [Identifying Outliers](#identifying-outliers)
  - [Label Encoding](#label-encoding)
- [Data Validation: The Why and What](#data-validation-the-why-and-what)
- [Joining Data and the Importance of Validation](#joining-data-and-the-importance-of-validation)
- [Essential Data Visualization Resources](#essential-data-visualization-resources)
- [Further Resources for Data Visualization](#further-resources-for-data-visualization)
- [Project overview: Automatidata](#project-overview-automatidata)
- [Project overview: Tiktok](#project-overview-tiktok)
- [Project overview: Waze](#project-overview-waze)
- [What is A/B Testing?](#what-is-ab-testing)
- [Statistical Concepts in A/B Testing](#statistical-concepts-in-ab-testing)
- [Understanding Central Tendency](#understanding-central-tendency)
- [Understanding Measures of Dispersion](#understanding-measures-of-dispersion)
- [Understanding Percentiles and Quartiles](#understanding-percentiles-and-quartiles)
- [Basic concepts of probability](#basic-concepts-of-probability)
- [Conditional Probability](#conditional-probability)
- [Bayes's Theorem Overview](#bayess-theorem-overview)
- [Discrete Probability Distributions](#discrete-probability-distributions)
- [Continuous Probability Distributions](#continuous-probability-distributions)
- [Z-Score](#z-score)
- [Understanding Population and Sample](#understanding-population-and-sample)
- [Representative Samples for Accurate Insights](#representative-samples-for-accurate-insights)




# Data Organization and Structure

A **database (DB) file** is a structured system for storing data, typically in tables, indexes, or fields that allow for efficient querying and retrieval. In contrast, a **CSV (Comma Separated Values)** file is a simpler, text-based format where data is stored in plain text, making it easy to read and exchange between different systems, but lacking the complexity and capabilities of a database.

**Data sorting** refers to arranging data in a meaningful order, often based on values or categories, to facilitate analysis. **Grouping** aggregates related data into categories or clusters, which is essential for summarizing data points and generating insights at a higher level.

# Data Sources and Types

**Data sources** refer to the origins of the data you're working with. These sources are commonly classified into:
- **First-party data**: Collected directly from your organization (e.g., customer data from your own website).
- **Second-party data**: Obtained directly from another organization (e.g., through partnerships or purchases).
- **Third-party data**: Aggregated from various external sources (e.g., market research firms).

In terms of **data types**, two common examples are:
- **Strings**: Represent textual data (e.g., names, addresses).
- **Integers**: Represent whole numbers, often used for counting or indexing (e.g., age, number of items sold).

# Data Analysis Concepts

**Extracting data** involves retrieving it from various sources—such as databases, APIs, or files—for the purpose of processing or storage in a more accessible format. **Filtering** narrows down datasets by selecting a specific subset of records based on given criteria, allowing analysts to focus on the most relevant data for their needs.

A **hypothesis** in data analysis is a testable proposition based on existing knowledge or observations. It provides a framework for testing relationships between variables and validating assumptions through further investigation and analysis.


# How to approach duplicates in data

Identifying duplicates involves using the duplicated() function in Pandas, which flags duplicate rows in a dataset.
Deciding whether to remove duplicates depends on the nature of the dataset and the analysis goals; sometimes, duplicates are errors, while other times, they represent valid data points.
Deduplicating Data using Python

Deduplication, the process of removing duplicate values, can be achieved using the drop_duplicates() function in Pandas.
This function allows for specifying subsets of columns to check for duplicates, providing flexibility in handling different scenarios.  

# What is Categorical Data?

Categorical data is information that is divided into groups, often represented with words rather than numbers, such as occupations or educational levels.
Many data models and algorithms struggle with categorical data in its raw form, making conversion to numerical data necessary.
Transforming Categorical Data

**Dummy Variables**: This method uses binary values (0 or 1) to represent the presence or absence of a specific category.

**Label Encoding**: This technique assigns a unique numerical value to each category, simplifying data processing and analysis. 

# Label Encoding Example

Imagine you have a 'Fruit' column in your dataset with these values:

```
Apple
Banana
Orange
Apple
Banana
```

Using label encoding, you would transform this column as follows:

- **Apple**: 0
- **Banana**: 1
- **Orange**: 2

The transformed 'Fruit' column would now look like this:

```
0
1
2
0
1
```

# Python Methods Overview

## Understanding Numerical Representation

This numerical representation allows machine learning models to effectively understand and process data, which is crucial for building accurate predictive models.

## Handling Missing Data

- **Filling Missing Values:**  
  The `df.fillna()` method is useful for filling in missing values using a specified strategy, such as forward filling or backward filling.
  
- **Removing Missing Values:**  
  The `df.dropna()` method allows you to remove rows or columns that contain missing values, which can help maintain the integrity of your dataset.

## Identifying Outliers

- **Descriptive Statistics:**  
  The `df.describe()` method provides insights into the distribution of your data, such as mean, median, and standard deviation, which can help identify potential outliers.
  
- **Visualizing Outliers:**  
  Visualizing your data with a boxplot is an effective way to identify outliers. You can generate boxplots using the `sns.boxplot()` function from the Seaborn library.

## Label Encoding

- **One-Hot Encoding:**  
  The `pd.get_dummies()` function is very useful for converting categorical variables into a set of binary columns, enabling machine learning algorithms to better interpret these features.
  
- **Label Encoding:**  
  The `LabelEncoder()` from scikit-learn is a helpful tool for transforming categorical labels into numeric codes. This method is often used to prepare data for machine learning models when there are ordinal relationships between categories.


# Data Validation: The Why and What

Validating data is crucial for making sound business decisions and improving the performance of complex models, as it helps identify and correct errors, ensuring data accuracy.
During validation, data professionals check for consistency in data format, range, and type, ensuring that all entries adhere to the same standards.
# Joining Data and the Importance of Validation

Joining involves augmenting data by incorporating values from other datasets, similar to a chef adding more ingredients to a recipe.
Before joining datasets, validation is essential to ensure that the formatting and data entries align, and that the data types are compatible, just as a chef would ensure the consistency and taste of new ingredients match the existing ones.


# Essential Data Visualization Resources

**Tableau**: Offers a variety of software packages, a comprehensive education and tutorial platform, a vast collection of sample visualizations, articles, blogs, and white papers.

**PowerBI**: Known for its popular software used globally for data visualization, it provides a free online version, guided learning, online workshops, and a growing community of data professionals.

# Further Resources for Data Visualization

**Information is Beautiful**: A platform that showcases data visualizations on various topics, offers blogs, newsletters, workshops, and emphasizes transparency by sharing datasets used for their visualizations.

**Storytelling with Data**: Focuses on effective data communication, providing training, workshops, tools, and an engaged community for learning and feedback.

# Project overview: Automatidata

Automatidata works with its clients to transform their unused and stored data into useful solutions, such as performance dashboards, customer-facing tools, strategic business insights, and more. They specialize in identifying a client’s business needs and utilizing their data to meet those business needs. 

Automatidata is consulting for the New York City Taxi and Limousine Commission (TLC). New York City TLC is an agency responsible for licensing and regulating New York City's taxi cabs and for-hire vehicles. The agency has partnered with Automatidata to develop a regression model that helps estimate taxi fares before the ride, based on data that TLC has gathered. 

The TLC data comes from over 200,000 taxi and limousine licensees, making approximately one million combined trips per day. 

**Project background**

Automatidata is working on the TLC project. The following tasks are needed before the team can begin the data analysis process:

- EDA and cleaning

- Select and build visualization(s) type

- Create plots to visualize relationships between relevant variables
- Share your results with the Automatidata team

**Specific project deliverables**

complete the following deliverables:

- Course 3 PACE Strategy Document to consider questions, details, and action items for each stage of the project scenario

- Answer the questions in the Jupyter notebook project file

- Create a Jupyter notebook of full EDA

- Create a Tableau visualization showing two important variables

- Write an executive summary of results and include a visualization

# Project overview: Tiktok

At TikTok, our mission is to inspire creativity and bring joy. Our employees lead with curiosity and move at the speed of culture. Combined with our company's flat structure, you'll be given dynamic opportunities to make a real impact on a rapidly expanding company and grow your career.

TikTok users have the ability to submit reports that identify videos and comments that contain user claims. These reports identify content that needs to be reviewed by moderators. The process generates a large number of user reports that are challenging to consider in a timely manner. 

TikTok is working on the development of a predictive model that can determine whether a video contains a claim or offers an opinion. With a successful prediction model, TikTok can reduce the backlog of user reports and prioritize them more efficiently.

**Project background**

Automatidata is working on the TLC project. The following tasks are needed before the team can begin the data analysis process:

- EDA and cleaning

- Select and build visualization(s) type

- Create plots to visualize relationships between relevant variables
- Share your results with the Automatidata team

**Specific project deliverables**

complete the following deliverables:

- Course 3 PACE Strategy Document to consider questions, details, and action items for each stage of the project scenario

- Answer the questions in the Jupyter notebook project file

- Create a Jupyter notebook of full EDA

- Create a Tableau visualization showing two important variables

- Write an executive summary of results and include a visualization


# Project overview: Waze

Waze’s free navigation app makes it easier for drivers around the world to get to where they want to go. Waze’s community of map editors, beta testers, translators, partners, and users helps make each drive better and safer. Waze partners with cities, transportation authorities, broadcasters, businesses, and first responders to help as many people as possible travel more efficiently and safely. 

You’ll collaborate with your Waze teammates to analyze and interpret data, generate valuable insights, and help leadership make informed business decisions. Your team is about to start a new project to help prevent user churn on the Waze app. Churn quantifies the number of users who have uninstalled the Waze app or stopped using the app. This project focuses on monthly user churn. 

This project is part of a larger effort at Waze to increase growth. Typically, high retention rates indicate satisfied users who repeatedly use the Waze app over time. Developing a churn prediction model will help prevent churn, improve user retention, and grow Waze’s business. An accurate model can also help identify specific factors that contribute to churn and answer questions such as: 

Who are the users most likely to churn?

Why do users churn? 

When do users churn? 

For example, if Waze can identify a segment of users who are at high risk of churning, Waze can proactively engage these users with special offers to try and retain them. Otherwise, Waze may lose these users without knowing why. 

Your insights will help Waze leadership optimize the company’s retention strategy, enhance user experience, and make data-driven decisions about product development.

**Project background**

Automatidata is working on the TLC project. The following tasks are needed before the team can begin the data analysis process:

- EDA and cleaning

- Select and build visualization(s) type

- Create plots to visualize relationships between relevant variables
- Share your results with the Automatidata team

**Specific project deliverables**

complete the following deliverables:

- Course 3 PACE Strategy Document to consider questions, details, and action items for each stage of the project scenario

- Answer the questions in the Jupyter notebook project file

- Create a Jupyter notebook of full EDA

- Create a Tableau visualization showing two important variables

- Write an executive summary of results and include a visualization



# What is A/B Testing?

- A/B testing is a method used to compare two versions of something (like a webpage or an email) to determine which one performs better based on specific metrics.
- Businesses use A/B testing to optimize their products and improve customer experience by making data-informed decisions.
# Statistical Concepts in A/B Testing

- **Sampling**: Involves selecting a smaller group (a sample) from a larger population. A/B testing uses samples to make inferences about the entire user base.
- **Statistical Significance**: Helps determine if the observed differences between versions A and B are due to actual changes or random chance, ensuring that decisions are based on meaningful results.

# Understanding Central Tendency

Measures of central tendency help you understand the central point of a dataset, providing a single value that represents the typical value.
The mean is the average, the median is the middle value when ordered, and the mode is the most frequent value.
- **Mean vs. Median**

The mean is greatly affected by outliers (extreme values), while the median is more resistant to them.
Use the median when outliers are present, as it gives a more accurate representation of the typical value in such cases.

- **Using the Mode**

The mode is particularly useful for categorical data (like survey responses) as it highlights the most common category.
For example, in a survey on employee satisfaction, the mode would show the most frequent response, giving insights into overall sentiment.

# Understanding Measures of Dispersion

- **Range**: This is the simplest measure, calculated by subtracting the smallest value from the largest value in your dataset. It gives a quick snapshot of the data spread.
  
- **Variance and Standard Deviation**: Variance represents the average squared difference of each data point from the mean. Standard deviation, a more interpretable measure, is calculated as the square root of the variance.
  
**Practical Application of Standard Deviation**

Real Estate Example: Standard deviation helps understand price variations. For instance, two neighborhoods might have the same average rent, but different standard deviations. A higher standard deviation indicates a wider price range in that neighborhood.

# Understanding Percentiles and Quartiles

- A percentile reveals the percentage of data falling below a specific value, dividing data into 100 equal parts for relative positioning.
- Quartiles divide data into four equal parts, with Q1, Q2 (the median), and Q3 representing the 25th, 50th, and 75th percentiles, respectively.

  
**Interquartile Range (IQR) and Five Number Summary**

- The IQR represents the range between the first and third quartiles (Q3 - Q1), indicating the spread of the middle 50% of the data.
- The five-number summary (minimum, Q1, median/Q2, Q3, maximum) provides a concise overview of the data's distribution.


# Basic concepts of probability

**Types of Events**

- Mutually Exclusive Events
These events cannot happen simultaneously. Think of flipping a coin – you can't land on both heads and tails in one toss.

- Independent Events
The outcome of one event doesn't impact the other. Rolling a die twice exemplifies this, as the first roll doesn't influence the second.

**Rules of Probability**

- Complement Rule
This rule helps determine the probability of an event NOT happening. It's based on the idea that the probability of an event occurring plus the probability of it not occurring always equals 1.

- Addition Rule (for mutually exclusive events)
Use this to find the probability of either one event OR another happening. You simply add the probabilities of each individual event.

- Multiplication Rule (for independent events)
This rule comes in handy when you want to know the probability of two events happening one AFTER the other. You calculate this by multiplying the probabilities of each individual event.

# Conditional Probability
conditional probability refers to the probability of an event occurring given that another event has already occurred. For example, when you draw an ace from a deck of playing cards, this changes the probability of drawing a second ace from the same deck. 

# Bayes's Theorem Overview

Bayes's theorem is a statistical method that updates the probability of an event based on new information. It differentiates between two types of probabilities:

- **Prior Probability**: The initial probability of an event before new data is considered.
- **Posterior Probability**: The updated probability of an event after incorporating new data.

Bayes's theorem enables the calculation of posterior probability by adjusting prior probability with new evidence. For example, in a medical context, if a condition is associated with age, you can determine the probability of a person having that condition based on their age group, transforming the prior probability into a more accurate posterior probability.

## The Theorem

Bayes's theorem states:

$$ P(A|B) = \frac{P(B|A) \cdot P(A)}{P(B)} $$


Where:
- \(P(A|B)\): Posterior probability (the probability of event A given event B).
- \(P(B|A)\): Likelihood (the probability of event B given event A).
- \(P(A)\): Prior probability (the probability of event A).
- \(P(B)\): Evidence (the probability of event B).

In simpler terms, the theorem can be restated as:

**Posterior = Likelihood * Prior / Evidence**

This theorem allows for the transformation of prior beliefs into updated probabilities by incorporating new data, thereby providing a more accurate assessment based on relevant evidence.

# Discrete Probability Distributions

Discrete probability distributions describe the probabilities of the outcomes of a discrete random variable, which can take on a countable number of values. These distributions are essential in statistics and probability theory for modeling various real-world scenarios.

## Common Discrete Distributions

- **Uniform Distribution**: Imagine rolling a fair die. Each face (1-6) has an equal chance of landing face up. That's a uniform distribution - all outcomes are equally likely.

- **Binomial Distribution**: Think of flipping a coin multiple times. Each flip is independent (one flip doesn't affect the next). The binomial distribution helps us calculate the probability of getting a specific number of heads (or tails) in a set number of flips.

- **Bernoulli Distribution**:  This is like a single flip in our coin example. It represents the probability of success or failure in a single trial.  

- **Poisson Distribution**: Imagine you work at a call center. The Poisson distribution helps you predict the probability of receiving a specific number of calls within an hour, knowing the average number of calls you get per hour.

# Continuous Probability Distributions

- Unlike discrete variables with distinct values, continuous variables can take on any value within a range, represented by a curve called a Probability Density Function (PDF).
- The probability of a continuous variable falling within a specific interval is represented by the area under the curve (PDF) for that interval.
  
**The Normal Distribution**

- The normal distribution, also known as the bell curve, is symmetrical with the mean at its center.
- The empirical rule helps us understand the spread of data in a normal distribution: 68% within one standard deviation, 95% within two, and 99.7% within three.
- 
**Significance of the Normal Distribution**

- The normal distribution is frequently observed in real-world datasets, making it a valuable tool for data professionals.
- Understanding it is crucial for advanced statistical analyses like hypothesis testing and regression analysis.

# Z-Score

## Definition

The **z-score**, also known as the standard score, measures the number of standard deviations a data point is from the mean of a dataset. It provides a way to understand how a specific value compares to the average value in a distribution.

The formula for calculating the z-score of a value \(X\) is:

$$\[ 
z = \frac{(X - \mu)}{\sigma} 
\]$$

Where:
- $$\(X\)$$ = the value for which you are calculating the z-score.
- $$\(\mu\)$$ = the mean of the dataset.
- $$\(\sigma\)$$ = the standard deviation of the dataset.

## Purpose of Z-Score

1. **Standardization**: Z-scores standardize different datasets, making them comparable. For example, if you have scores from different tests with different scales, converting them to z-scores allows for direct comparison.

2. **Identifying Outliers**: Z-scores help identify outliers in a dataset. Generally, a z-score greater than 3 or less than -3 may indicate that a value is an outlier.

3. **Probability Calculations**: In a normal distribution, z-scores can be used to determine probabilities and percentiles. For instance, you can use z-scores to find the likelihood that a given value falls below or above a specific threshold in a normally distributed dataset.

4. **Data Interpretation**: Z-scores provide a way to interpret how far away a data point is from the mean. A positive z-score indicates the value is above the mean, while a negative z-score indicates it is below the mean.

# Understanding Population and Sample

A **population** in statistics refers to the entire group you want to study, while a **sample** is a smaller, representative subset of that population.

Data professionals often work with samples because collecting data from an entire population can be impractical, time-consuming, and expensive.

## Representative Samples for Accurate Insights

A representative sample accurately reflects the characteristics of the population, ensuring that conclusions drawn from the sample are applicable to the entire population. 

Non-representative samples can lead to inaccurate conclusions and predictions, highlighting the importance of using appropriate sampling methods to minimize bias.















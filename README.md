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


# Data Organization and Structure

A database (DB) file is used for storing data, often in tables, indexes, or fields, while a CSV file is a simpler format for storing data in plain text.
Data can be sorted, which means arranging it meaningfully for analysis, and grouped, which involves aggregating individual observations into groups.

# Data Sources and Types

Data sources refer to the origin of data, and they can be categorized as first-party (from your organization), second-party (directly from another organization), or third-party (aggregated data from various sources).
Strings and integers are common data types used in programming and data analysis. Strings represent textual information, while integers represent whole numbers.

# Data Analysis Concepts

Extracting involves retrieving data from sources for processing or storage, while filtering involves selecting a subset of data based on specific criteria.
A hypothesis is a testable explanation based on evidence, guiding further investigation and analysis.

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











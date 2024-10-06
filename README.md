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
- [Project overview: Automatidata](#Project-overview:-Automatidata)


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














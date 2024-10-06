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

![](data:image/png;base64,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)


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
















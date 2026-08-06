# Uber-Data-Analysis-Project

Here is a concise summary and overview prepared directly from your notebook:

Uber Data Analysis Project Overview
1. Dataset Summary
Initial Shape: 1,156 rows, 7 columns (START_DATE, END_DATE, CATEGORY, START, STOP, MILES, PURPOSE).

Cleaned Shape: 413 rows, 10 columns (after removing missing datetime entries and adding feature columns).

2. Data Preprocessing Steps
Missing Values: Filled missing PURPOSE values with "NOT".

Datetime Conversion: Converted START_DATE and END_DATE to datetime objects.

Feature Engineering:

Extracted date and time (hour) from START_DATE.

Categorized time into time bins (day-night: Morning, Afternoon, Evening, Night).

Extracted MONTH and mapped month numbers to names (e.g., Jan, Feb).

Extracted DAY of the week (e.g., Mon, Tues, Fri).

Cleaning: Dropped remaining NaN rows.

3. Key Insights & Visualizations
Categories & Purpose: The vast majority of trips are under the Business category, with Meetings and Meal/Entertainment being top purposes.

Time Profile: Most rides occur during the Afternoon and Evening periods.

Day Profile: Friday has the highest ride frequency, followed closely by Thursday.

Trip Distance Analysis:

Most trips are short-distance (under 10 miles).

Boxplots reveal significant long-distance outliers (up to 175+ miles).

Distribution plot confirms a right-skewed pattern peaked around 2–5 miles.

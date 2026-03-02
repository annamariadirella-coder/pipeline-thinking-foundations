# Reflection

A data pipeline, in my own words, is a structured process that moves data from a raw state to a clean and usable state. It is not only about writing code, but about understanding where data comes from, what problems it has, and what transformations are necessary to make it reliable for analysis or decision-making.

Raw data is often not ready for analysis because it is inconsistent, incomplete, or duplicated. Different systems store data in different formats, use different field names, or represent the same information in different ways. Without cleaning and standardizing the data, any analysis based on it could lead to incorrect conclusions.

The easiest scenario for me was the Online Orders CSV because the problems were clear and common, such as duplicates and inconsistent formatting. The most challenging scenario was the Retail Product Data because it required thinking about multiple suppliers, different file formats, currency conversion, and product matching. It involved more complex integration logic.

One important thing I learned from this exercise is that data engineering starts with thinking clearly about structure and consistency. Before writing any code, it is essential to understand the data flow, the transformations required, and the final expected output.

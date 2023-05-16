# PandasAI
## Empowering Data Scientists and Analysts: Simplifying Data Analysis with OpenAI's Pandas AI, the Generative Python Library

Pandas AI is a Python library that integrates generative AI capabilities into Pandas, a widely used data manipulation and analysis toolkit. This library takes your data analysis to the next level by making data frames conversational, meaning you can interact with your data set and receive immediate responses. This project is powered by OpenAI and provides a revolutionary way to simplify data analysis for data scientists and analysts.

### Introduction
Data scientists and analysts often spend considerable time preparing data for analysis. Pandas AI, a novel addition to the data science toolbox, seeks to minimize this time by allowing users to directly converse with their data. By integrating with the OpenAI API, Pandas AI enables users to ask questions about their data and receive answers in the form of Pandas DataFrames. The tool is designed to be used alongside the traditional Pandas library, not as a replacement.

### How to use
To install Pandas AI, use pip:
```
pip install pandasai
```


To use Pandas AI, you need to import PandasAI and OpenAI, and then initialize an OpenAI model with your API key:

```
 import pandas as pd
 from pandasai import PandasAI
 from pandasai.llm.openai import OpenAI
 ```

### Instantiate a LLM
```
 from pandasai.llm.openai import OpenAI
 llm = OpenAI(api_token="your_api_key")
 pandas_ai = PandasAI(llm, conversational=False)
 ```

If you don't have an OpenAI API key, you can create an account on the OpenAI platform and generate an API key.

Next, 
### Run the model on your data frame
```
pandas_ai.run(df, prompt='the question you would like to ask?')
```
### Example
open `PandasAI.ipynb` to see example

### License
PandasAI is licensed under the MIT License. See the LICENSE file for more details.

# Working with `pandas`

[pandas](https://pandas.pydata.org/) is a fast, powerful, flexible and easy to use open source data analysis and
manipulation tool, built on top of the Python programming language. [1]

![pandas](https://upload.wikimedia.org/wikipedia/commons/thumb/e/ed/Pandas_logo.svg/768px-Pandas_logo.svg.png?20200209204934)

The most relevant benefits are:

* Easy-to-use interface
* Fast tabular data manipulation
* Lot of flexibility working with tables
    * Even the complex ones

## How to install `pandas` library?

> To install pandas just execute the following command: `pip install pandas

## Examples
Here is an example of code with pandas:
```
import pandas as pd

# read csv data
data = pd.read_csv("./files/mydata.csv")
data = data.dropna()

# write csv
data.write_csv("./files/processed_data.csv")
```
---
[1]: Go [here](https://pandas.pydata.org/docs/getting_started/index.html#getting-started) to start using pandas ↩️



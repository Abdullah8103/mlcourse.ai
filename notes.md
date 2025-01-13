
# main Pandas methods

<p>With this we can import numpy<br><strong>import numpy as np</strong></p>
<p>With this we can import pandas<br><strong>import pandas as pd</strong></p>
<p><strong>pd.set_option("display.precision", 2)</strong></p>
<p>Import csv into a panda dataframe<br><strong>df = pd.read_csv("../../data/telecom_churn.csv")</strong></p>
<p>Show the top 5 entries in the dataframe<br><strong>df.head()</strong></p>
<p>Show shape of the dataframe as<br><strong>df.shape()</strong></p>
<p>Show names of the coloumns of the dataframe as<br><strong>df.columns()</strong></p>
<p>Show information of the coloumns of the dataframe as<br><strong>df.info()</strong></p>
<p>Change the datatype of one of the columns by<br><strong>df[column name] = df[column name].astype(type)</strong></p>
<p>describe the data ( and include specific data types )<br><strong>df.describe(include=["object", "bool"])</strong></p>
<p>describe the the value counts of a specific series<br><strong>df[column name].value_counts(normalize = true))</strong></p>

# sorting data frames
<p>Sorting a dataframe<br><strong>df.sort_values(by=["Churn", "Total day charge"], ascending=False).head()</strong></p>

# Indexing and retrieving data
<p>You can index by doing the array thing<br><strong>df[column name]</strong></p>
<p>You can index by using a condition<br><strong>df.select_dtypes(include=np.number)[df["Churn"] == 1].mean()</strong></p>
<p>You can index with loc<br><strong>df.loc[0:5, "State":"Area code"]</strong></p>
<p>You can index with iloc<br><strong>df.iloc[0:5, 0:3]</strong></p>

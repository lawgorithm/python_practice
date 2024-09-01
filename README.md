# python_practice

* **Filtering**
  * df.drop_duplicates()
    * [30 Days of Pandas.ipynb](https://github.com/lawgorithm/python_practice/blob/main/30_Days_of_Pandas.ipynb)
  * df.rename(columns={'old_name': 'new_name'})
    * [30 Days of Pandas.ipynb](https://github.com/lawgorithm/python_practice/blob/main/30_Days_of_Pandas.ipynb)
  * df.sort_values(by=['id'], ascending=True)
    * [30 Days of Pandas.ipynb](https://github.com/lawgorithm/python_practice/blob/main/30_Days_of_Pandas.ipynb)
  * df[df['id'].isin(df['other_id'])]
    * [30 Days of Pandas.ipynb](https://github.com/lawgorithm/python_practice/blob/main/30_Days_of_Pandas.ipynb)
   
* **Column manipulations**
  * series.apply()
    * [30 Days of Pandas.ipynb](https://github.com/lawgorithm/python_practice/blob/main/30_Days_of_Pandas.ipynb)
    * Example: df['some_string'].apply(len)
      * This can product a new column that counts the char length of each entry in the 'some_string' column. We pass the function len() to the apply method.
  * series.isna()
    * [30 Days of Pandas.ipynb](https://github.com/lawgorithm/python_practice/blob/main/30_Days_of_Pandas.ipynb)
    * Example: df['customerId'].isna()
      * Can help you select columns that are or are not NA

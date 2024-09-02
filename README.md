# python_practice

* **DF Initialization**
  * df = pd.DataFrame({f'col1': [val0, ..., valn]})
    * [30 Days of Pandas.ipynb](https://github.com/lawgorithm/python_practice/blob/main/30_Days_of_Pandas.ipynb)

* **DF Indexing**
  * df.loc[row_cond, col]
    * [30 Days of Pandas.ipynb](https://github.com/lawgorithm/python_practice/blob/main/30_Days_of_Pandas.ipynb)

* **Series Filtering**
  * df.drop_duplicates()
    * [30 Days of Pandas.ipynb](https://github.com/lawgorithm/python_practice/blob/main/30_Days_of_Pandas.ipynb)
  * df.rename(columns={'old_name': 'new_name'})
    * [30 Days of Pandas.ipynb](https://github.com/lawgorithm/python_practice/blob/main/30_Days_of_Pandas.ipynb)
  * df.sort_values(by=['id'], ascending=True)
    * [30 Days of Pandas.ipynb](https://github.com/lawgorithm/python_practice/blob/main/30_Days_of_Pandas.ipynb)
  * df[df['id'].isin(df['other_id'])]
    * [30 Days of Pandas.ipynb](https://github.com/lawgorithm/python_practice/blob/main/30_Days_of_Pandas.ipynb)
   
* **Column/Series manipulations**
  * Series.apply()
    * [30 Days of Pandas.ipynb](https://github.com/lawgorithm/python_practice/blob/main/30_Days_of_Pandas.ipynb)
    * Example: df['some_string'].apply(len)
      * This can product a new column that counts the char length of each entry in the 'some_string' column. We pass the function len() to the apply method.
  * Series.isna()
    * [30 Days of Pandas.ipynb](https://github.com/lawgorithm/python_practice/blob/main/30_Days_of_Pandas.ipynb)
    * Example: df['customerId'].isna()
      * Can help you select columns that are or are not NA
  * Series.str.contains(pattern)
    * [30 Days of Pandas.ipynb](https://github.com/lawgorithm/python_practice/blob/main/30_Days_of_Pandas.ipynb)
    * Example: df['conditions'].str.contains(r'(^DIAB1)|( DIAB1)')
      * Vector of booleans
  * Series.str.fullmatch(pattern)
    * [30 Days of Pandas.ipynb](https://github.com/lawgorithm/python_practice/blob/main/30_Days_of_Pandas.ipynb)
    * Example: df['mail'].str.fullmatch(r'^[a-zA-Z][a-zA-Z0-9_.-]*@leetcode\.com')
      * Vector of booleans
  * Series.drop_duplicates()
    * [30 Days of Pandas.ipynb](https://github.com/lawgorithm/python_practice/blob/main/30_Days_of_Pandas.ipynb)
    * Example (unique sorted salaries): df['salary'].drop_duplicates().sort_values(ascending=False)
  * Series.rank()
    * [30 Days of Pandas.ipynb](https://github.com/lawgorithm/python_practice/blob/main/30_Days_of_Pandas.ipynb)
    * Example (reverse ranks -- dense mean [1,2,2,3] instead of [1,2,2,4]. Use 'min' for the latter): df['score'].rank(method='dense', ascending = False)
* **Column/Series Indexing**
  * Series.iloc[N]
    * [30 Days of Pandas.ipynb](https://github.com/lawgorithm/python_practice/blob/main/30_Days_of_Pandas.ipynb)

* `np.isnan(X[:, i].astype(float)).any()` tells if there is NaN in **i**th column of X, X being ndarray (type can be changed acc. to the datatype, here it is float)

* `train_df.iloc[:, i].isnull().values.any()` tells if there is NaN in **i**th column of train_df, train_df being dataframe

* `train_df.iloc[:, i].isnull().values.sum()` tells number of NaN in **i**th column of train_df, train_df being dataframe

* `np.where(pd.isnull(train_df.iloc[:, i]))` tells where NaN is located in train_df, train_df being dataframe

* `train_df.columns.get_loc("pear")` tells the index of column by name "pear"

* ```
  corr = train_df.corr()["target_variable_name"]
  corr[np.argsort(corr, axis=0)[::-1]]
  ``` 
	tells the correlation between features and the target variable, 1.00 being the highest. ('-1' for arranging in decreasing order)

* `np.delete(arr_name, col/row_index, axis)`	deletes row/col of specified index along specified axis = 0 for horizontal and axis = 1 for vertical)

* ```
  for i in range(0,num_of_col) :
	print(str(i) + ' index col : ' + str(train_df.iloc[:, i].isnull().values.any()) + '('+ str(train_df.columns[i]) +')')
  ``` 
	tells if there is NaN in each column(or feature) of dataframe with col. name and index

* `train_df['col'].unique()	` gives unique values of column with name 'col' from train_df dataframe

* `df.groupby('col_1')['unique_id'].nunique()`	gives count of unique values in 'col_1' where each row in uniquely	identified by 'unique_id'

* `df['col_1'].value_counts()` same as above

* `df.iloc[:, i].value_counts()` same as above except it uses index 'i'
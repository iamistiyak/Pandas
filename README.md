# Pandas Tutorial

**Description:** I have created this full pandas tutorial for get insight about overall pandas functionality in the project.<br>
                 All the processing files uploaded uder the **Resource** folder<br><br>

I have created this jupyter notebook to cover the pandas topics in concise manner.<br><br>

| Serial | Topics | 
| :--- | --- |
| 01 | Reading in files |
| 02 | Filtering and ordering |
| 03 | Indexing |
| 04 | Grouping and aggregate |
| 05 | Merging data frame|
| 06 | Visulization in pandas |
| 07 | Data cleaning in pandas |
| 08 | Exploratory data analysis |<br><br><br><br>

I have used this command for fulfil the above purposes.
| Command | Description |
| :--- | --- |
| df.read_csv | Read the csv files |
| df.read_excel | Read the excel files |
| df.read_table | Read text file as a table form |
| pd.set_option('display.max.rows', 235)| Can see the all the rows |
| df.head(10) | Show the 1st 10 rows |
| df.tail(10) | Show the last 10 rows |
| df[“ColName”] | Show the specific column |
| df2.loc["United States"] | For string location |
| df2.iloc[3] | For integer location. |
| isin | specific_countries = ["India", "Pakistan"] <br>df[df['Country'].isin(specific_countries)]|
| str.contain | Show the values contained United <br> df[df['Country'].str.contains('United')] |
| df.set_index('Country') | Set the index of the data frame |
| df. filter() | df2.filter(items = ['Continent', 'CCA3']) |
| Axis =1 -> Column <br> Axis = 0 -> Row | df2.filter(items = ['Continent', 'CCA3'], axis = 1) <br>  df2.filter(items = ['India'], axis = 0) |
| sort_values | df[df["Rank"]<10].sort_values(by="Rank") <br> df[df["Rank"]<10].sort_values(by=["Rank","Country"], ascending = False) <br> df[df["Rank"]<10].sort_values(by=["Continent","Country"], ascending = [True, False] ) |
| Index_col | df = pd.read_csv(r”c:\etc.”, index_col= "Country") |
| reset_index | df.reset_index(inplace=True) |
| set_index | df.set_index("Country") <br> df.set_index(["Continent","Country"], inplace=True) <br> df.sort_index(ascending=[False,True]) |
| df.groupby | group_by_frame = df.groupby('Base Flavor') |
| mean() | Calculate the mean values <br>group_by_frame.mean() |
| count() | df.groupby('Base Flavor').count() |
| min() | df.groupby('Base Flavor').min() |
| max() | df.groupby('Base Flavor').max() |
| sum() | df.groupby('Base Flavor').sum() |
| agg() | Multiple operation in a line <br>df.groupby('Base Flavor').agg({'Flavor Rating': ['mean', 'max', 'count', 'sum']}) |
| describe() | Describe the data frame |
| merge() | df1.merge(df2)<br> df1.merge(df2, how = "inner", on = "FellowshipID") <br>df1.merge(df2, how = "inner", on = ["FellowshipID", "FirstName"])<br> df1.merge(df2, how = "cross") |
| join() | df4 = df1.set_index('FellowshipID').join(df2.set_index('FellowshipID'), lsuffix='_Left', rsuffix = '_Right') |
| Concat() | pd.concat([df1,df2]) <br> pd.concat([df1,df2], join = 'outer', axis = 1) |

<br><br>
| Special Command | Description |
| :--- | --- |
| Shift + Tab | To open the description of the all functions under the formula. |
| Html Commands  | It is basically used for design the Jupyter notebook <br>  h1 style = "color:Green:.  For heading <br> u ":.  For underline <br> "<b >":.  For bold text |
| Shift + Enter  | Read the excel files |
| Html Commands  |Save and run the code  |

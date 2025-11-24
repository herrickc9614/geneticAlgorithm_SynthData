Clicking "Open in Colab" will open the file within Google Colab

Clicking Run all will compile each cell
-This will result in the Diabetes Dataset to be used-

If the loan approval dataset is desired, only run those cells and skip to dividing the datasets
If a non-included dataset is desired, load the csv file in the following way

#replace file path with you csv's filepath
df = pd.read_csv("filePath")

df.drop_duplicates()
df.info()

df.info will provide information on your dataset such as total size, collumn names, and data in each collum.

divide the collumns contained within your csv into the following

X = df[['collumn Name']]
y = df[['collumn Name']]

X should contain all collumns needed to create predictions
Y should only contain the collumn you want to predict

The rest of the code should adjust after these changes

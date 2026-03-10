# EXNO-6-DS-DATA VISUALIZATION USING SEABORN LIBRARY

# Aim:
  To Perform Data Visualization using seaborn python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:
 import seaborn as sns

df=sns.load_dataset("iris")

df.head()

<img width="734" height="235" alt="Screenshot 2026-03-10 112045" src="https://github.com/user-attachments/assets/340a18d2-a315-480c-87b9-14159adc281c" />

df.corr(numeric_only=True)

<img width="616" height="204" alt="Screenshot 2026-03-10 112101" src="https://github.com/user-attachments/assets/d64c340e-34c8-4aad-b899-7b7dc5c28206" />

sns.heatmap(df.corr(numeric_only=True))

<img width="527" height="418" alt="image" src="https://github.com/user-attachments/assets/fa33051d-80dd-4b52-931e-2856cefcdf53" />

sns.jointplot(x='petal_length',y='petal_width',data=df,kind='hex')

<img width="589" height="590" alt="image" src="https://github.com/user-attachments/assets/e86b0296-1579-4394-8bb5-1bae2bee0761" />

sns.jointplot(x='petal_length',y='petal_width',data=df,kind='reg')

<img width="589" height="590" alt="image" src="https://github.com/user-attachments/assets/78eed6b4-cdbb-4f7a-806b-4ccd4ab64424" />

sns.pairplot(df)

<img width="986" height="986" alt="image" src="https://github.com/user-attachments/assets/8944ca2a-a796-425c-a2f7-8c50c728cae2" />

sns.pairplot(df,hue='sepal_length')

<img width="846" height="741" alt="image" src="https://github.com/user-attachments/assets/6b47045a-557e-4134-98e1-a8bedc99b9b5" />

sns.distplot(df['petal_length'])

<img width="576" height="433" alt="image" src="https://github.com/user-attachments/assets/4deeec9a-0efc-4ec7-97ae-486abb7fd1a2" />

sns.distplot(df['petal_length'],kde=False,bins=10)

<img width="543" height="433" alt="image" src="https://github.com/user-attachments/assets/bd8b045d-66ff-414b-9cd7-b2662a74c686" />

sns.countplot(x='petal_length',data=df)

<img width="568" height="433" alt="image" src="https://github.com/user-attachments/assets/06e0124e-efa4-416a-abff-ceef0b2beb75" />

sns.countplot(x='species',data=df)

<img width="562" height="432" alt="image" src="https://github.com/user-attachments/assets/8c03bfdc-39e1-4c08-96f5-0a7d837a74d1" />

sns.countplot(x='species',data=df)

<img width="562" height="432" alt="image" src="https://github.com/user-attachments/assets/5e48786c-fa5e-487e-9dda-524f18a9eb57" />

sns.barplot(x='petal_length',y='petal_width',data=df)

<img width="572" height="433" alt="image" src="https://github.com/user-attachments/assets/e6657cce-2343-4a7a-95ba-46701ef7e178" />

sns.barplot(x='petal_width',y='petal_length',data=df)

<img width="554" height="436" alt="image" src="https://github.com/user-attachments/assets/1c700699-3306-4e5a-b82a-de4b706e3cc6" />

df.head()

<img width="689" height="222" alt="Screenshot 2026-03-10 112549" src="https://github.com/user-attachments/assets/46188ac7-5567-46a2-818a-9e8a05e9ef80" />

sns.boxplot(x='species',y='sepal_length', data=df)

<img width="567" height="432" alt="image" src="https://github.com/user-attachments/assets/251820a3-e0de-48ab-9bef-05fd37cb6c3f" />

sns.boxplot(x="species", y="sepal_length", data=df,palette='rainbow')

<img width="567" height="432" alt="image" src="https://github.com/user-attachments/assets/def673cb-5c06-42f6-a7d5-4e4f2c7444e6" />

sns.boxplot(data=df,orient='v')

<img width="534" height="413" alt="image" src="https://github.com/user-attachments/assets/f3cbd249-4178-4fa6-b1ff-59bf74b6f0ae" />

sns.boxplot(x="sepal_length", y="species", hue="species",data=df)

<img width="614" height="433" alt="image" src="https://github.com/user-attachments/assets/0a5bb8a6-19d9-4483-8c97-7c70d568ae1e" />

sns.violinplot(x="sepal_length", y="species", data=df,palette='rainbow')

<img width="613" height="433" alt="image" src="https://github.com/user-attachments/assets/091abd11-3404-44cf-9daf-e6e17abfa0e6" />

# Result:
 Thus we performed Data Visualization using seaborn python library for the given datas.

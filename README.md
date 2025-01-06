# Data-cleaning-project
A python project to clean a sample dataset
import pandas as pd

# Load the dataset (make sure you upload a sample CSV file to your GitHub repo)
df = pd.read_csv('netflix_titles.csv')

# Show first few rows of the dataset
print("Original Data:")
print(df.head())

# Clean data: Remove rows with missing values
df_cleaned = df.dropna()

# Show the cleaned data
print("\nCleaned Data:")
print(df_cleaned.head())

# Save cleaned data to a new CSV
df_cleaned.to_csv('cleaned_data.csv', index=False)

print("\nCleaned data has been saved to 'cleaned_data.csv'")

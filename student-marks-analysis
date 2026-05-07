import pandas as pd
import matplotlib.pyplot as plt

# Read CSV file
file = pd.read_csv('students.csv')

# Display data
print("Student Data:\n")
print(file)

# Average marks
file['Average'] = (file['Maths'] + file['Science'] + file['English']) / 3

print("\nAverage Marks:\n")
print(file[['Name', 'Average']])

# Highest scorer
highest = file.loc[file['Average'].idxmax()]

print("\nTop Scorer:\n")
print(highest['Name'], '-', highest['Average'])

# Graph
file.plot(x='Name', y=['Maths', 'Science', 'English'], kind='bar')

plt.title('Student Marks Analysis')
plt.ylabel('Marks')

plt.show()

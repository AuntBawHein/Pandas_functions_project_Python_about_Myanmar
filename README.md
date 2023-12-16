# Pandas_functions_project_Python_about_Myanmar

Step 1: Title and Introduction
Title of the Report: Exploring Tuberculosis Patient Data in Myanmar using Pandas in Python
Introduction: 
This report focuses on utilizing the Pandas library in Python for the analysis and manipulation of tuberculosis patient data in Myanmar. 
Panda is a tool that facilitates data organization, manipulation, and visualization.

Step 2: Advantages and Use Cases
Advantages: Pandas offer several advantages, such as quick data organization and the creation of visual representations, making it a valuable tool for real-life situations, particularly in managing tuberculosis cases.

What can we use Pandas to do in Python? :
Pandas enable efficient organization, analysis, and visualization of data. 

In this project, it is used for tasks like data organization, mathematical analysis, and creating visual graphs.

1. When to use Pandas in Python? 
: Pandas is employed when specialized data analysis and manipulation are required. In this project, it is used to explore and understand various aspects of tuberculosis patient data in Myanmar.

3. Why do we use Pandas in Python?
. : Because Pandas is used to manage and analyze tuberculosis patient data, providing structured handling of complex datasets.

Step 3: Project Code
Project Code:
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt

# Creating a sample DataFrame with patient information
data = {
    'Serial number': [1, 2, 3, 4, 5],
    'Name': ['Aung Kyaw', 'Thida', 'Min Aung', 'Su Su', 'Htet Naing'],
    'Sex': ['M', 'F', 'M', 'F', 'M'],
    'Age': [40, 25, 32, 28, 35],
    'Days first symptoms - first visit': [7, 5, 10, 3, 8],
    'Days first visit - diagnostic': [3, 2, 5, 1, 4],
    'Days diagnostic - outcome': [14, 12, 16, 8, 10],
    'Days first symptoms - outcome': [24, 19, 31, 12, 22]
}

# Creating a DataFrame using the provided data
df = pd.DataFrame(data)

# Creating a line graph with bubbles
plt.figure(figsize=(10, 6))

# Line plot for Days first symptoms - outcome
plt.plot(df['Serial number'], df['Days first symptoms - outcome'], marker='o', label='Symptoms to Outcome')

# Adding bubbles using Days first visit - diagnostic as bubble size
plt.scatter(df['Serial number'], df['Days first visit - diagnostic'], s=df['Days first visit - diagnostic']*10, c='red', label='Days Visit to Diagnostic')

# Adding labels and title
plt.xlabel('Patient Serial Number')
plt.ylabel('Number of Days')
plt.title('Follow-up of TB Patients (2020-2023)')
plt.legend()

# Showing the graph
plt.show()

These are questions and images here.
[Questions_and_image_Pandas_function_projects.docx](https://github.com/AuntBawHein/Pandas_functions_project_Python_about_Myanmar/files/13692274/Questions_and_image_Pandas_function_projects.docx)


And these are all Python codes sir, thank you very much.
[report_pandas_python_presentation (1).docx](https://github.com/AuntBawHein/Pandas_functions_project_Python_about_Myanmar/files/13692278/report_pandas_python_presentation.1.docx)



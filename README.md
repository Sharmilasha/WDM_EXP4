### EX4 Implementation of Cluster and Visitor Segmentation for Navigation patterns
### DATE: 
### AIM: To implement Cluster and Visitor Segmentation for Navigation patterns in Python.
### Description:
<div align= "justify">Cluster visitor segmentation refers to the process of grouping or categorizing visitors to a website, 
  application, or physical location into distinct clusters or segments based on various characteristics or behaviors they exhibit. 
  This segmentation allows businesses or organizations to better understand their audience and tailor their strategies, marketing efforts, 
  or services to meet the specific needs and preferences of each cluster.</div>
  
### Procedure:
1) Read the CSV file: Use pd.read_csv to load the CSV file into a pandas DataFrame.
2) Define Age Groups by creating a dictionary containing age group conditions using Boolean conditions.
3) Segment Visitors by iterating through the dictionary and filter the visitors into respective age groups.
4) Visualize the result using matplotlib.

### Program:
```
# read the data
import pandas as pd
visitor_df = pd.read_csv('/content/clustervisitor.csv')

# Perform segmentation based on characteristics (e.g., age groups)
age_groups = {
    'Young': visitor_df['Age'] <= 30,
    'Middle-aged': (visitor_df['Age'] > 30) & (visitor_df['Age'] <= 50),
    'Elderly': visitor_df['Age'] > 50
}

for group, condition in age_groups.items():  
    visitors_in_group = visitor_df[condition] 
    print(f"Visitors in {group} age group:")
    print(visitors_in_group)

```

### Output:

![image](https://github.com/Sharmilasha/WDM_EXP4/assets/94506182/4137c4d1-06c8-4eaf-9433-2156ab61c2e5)


### Visualization:
```python
# Create a list to store counts of visitors in each age group
/*WRITE YOUR CODE HERE

# Count visitors in each age group
/*WRITE YOUR CODE HERE
    
# Define age group labels and plot a bar chart
/*WRITE YOUR CODE HERE

plt.figure(figsize=(8, 6))
plt.bar(age_group_labels, visitor_counts, color='skyblue')
plt.xlabel('Age Groups')
plt.ylabel('Number of Visitors')
plt.title('Visitor Distribution Across Age Groups')
plt.show()
```
### Output:

![image](https://github.com/Sharmilasha/WDM_EXP4/assets/94506182/b3bec2ec-9c70-40a8-a1b0-5d24ec770f26)

### Result:
Thus the Implementation of Cluster and Visitor Segmentation for Navigation patterns is executed successfully.

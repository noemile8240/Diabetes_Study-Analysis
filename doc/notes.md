# Diabetes Risk Factor Analysis

This project explores a diabetes dataset with the goal of identifying key risk factors and generating meaningful insights through data exploration, SQL, and Tableau.

---

## Thought Process & Notes

### Project Goal  
My goal for this project was to explore the dataset, understand the story it was telling, and uncover impactful insights—especially around risk factors for diabetes.

### Data Understanding  
I used a dataset from a diabetes study published on Kaggle. Some initial data cleaning was required, and I maintained a changelog to document all modifications for transparency and traceability.

### Exploration & Insights  
I began by doing a quick review of the data in Excel to get a sense of the variables and general condition of the dataset. After that, I used SQL to clean the data and perform exploratory queries.

As I explored the data, I confirmed patterns I already suspected—such as the strong correlation between high glucose levels, high BMI, and diabetes. However, one insight that really surprised me was the role of age. The data showed that **age is the strongest factor** associated with diabetes risk. I had always assumed that if someone didn’t develop diabetes early in life, they likely wouldn’t later on. This dataset challenged that assumption.

After identifying correlations and key variables, I decided to focus the visualizations on identifying **risk factors** for diabetes.

### Design Decisions  
I chose simple bar charts and a clean, minimalist layout. I used a consistent color scheme across all visuals to help the viewer quickly recognize key categories:
- **Blue** to represent age  
- **Gray** for glucose groups  
- **Green** to indicate diabetes diagnosis

This approach kept the dashboard visually cohesive and easy to understand.

### Challenges  
The main challenge I encountered was the limited scope of the data. It only provided a single snapshot in time, which made it impossible to evaluate trends or changes over time. Despite this limitation, I focused on extracting as much insight as possible from the available metrics.

### Takeaways  
This project reinforced the importance of data exploration and hypothesis testing. I gained a clearer understanding of which health factors are most strongly associated with diabetes and how to visually communicate those relationships. It also reminded me how data can challenge our assumptions—and why it’s so valuable to investigate with an open mind.

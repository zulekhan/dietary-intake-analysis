# **Gender Differences in Dietary Intake**
![image](https://github.com/user-attachments/assets/84a90e96-7101-433c-bf83-2198cf264ed2)

## **Project Overview**
This project analyzes gender-based differences in dietary intake using data from the **National Health and Nutrition Examination Survey (NHANES)**. The goal is to determine whether males and females have significantly different consumption patterns for **calories, protein, carbohydrates, and fats**.

### **Research Questions**
1. Do males and females consume different amounts of **total calories**?
2. Are there significant differences in **protein, carbohydrate, and fat intake** between genders?
3. What insights can be drawn from dietary trends, and how might they inform public health recommendations?

---

## **Methodology**
1. **Data Collection**: We used two datasets from NHANES, available on Kaggle.
2. **Data Cleaning & Merging**: We filtered and combined the datasets based on participant ID (`SEQN`).
3. **Exploratory Data Analysis (EDA)**: We computed summary statistics and visualized data using bar plots and boxplots.
4. **Statistical Testing**: We conducted an **independent t-test** to compare dietary intake between males and females.
5. **Interpretation & Discussion**: We evaluated findings and suggested potential implications.

---

## **Datasets Used**
| Dataset | Description | Link |
|---------|------------|------|
| **Demographic Data** (`demographic.csv`) | Contains participant information, including gender. | [Download Here](https://www.kaggle.com/datasets/cdc/national-health-and-nutrition-examination-survey?resource=download&select=demographic.csv) |
| **Dietary Data** (`diet.csv`) | Contains daily food intake details, including calorie and macronutrient consumption. | [Download Here](https://www.kaggle.com/datasets/cdc/national-health-and-nutrition-examination-survey?resource=download&select=diet.csv) |

---

## **Data Dictionary**
This table explains the key variables used in this analysis.

| **Column Name** | **Description** |
|---------------|--------------------------------------|
| `SEQN`       | Unique participant ID |
| `RIAGENDR`   | Gender of the participant (1 = Male, 2 = Female) |
| `Gender`     | Mapped gender label (Male or Female) |
| `DR1TKCAL`   | Total calorie intake (kcal) |
| `DR1TPROT`   | Total protein intake (grams) |
| `DR1TCARB`   | Total carbohydrate intake (grams) |
| `DR1TTFAT`   | Total fat intake (grams) |



## **How to Set up and Run This Notebook**
This project was developed using **Jupyter Notebook** with **Python 3.12.6** (ipykernel). All necessary dependencies are listed in the `requirements.txt` file.

### **Steps to Set Up and Run the Project**

1. **Clone the Repository**:  
   Clone the repository to your local machine:  
   ```bash
   git clone <your-repo-link> && cd <your-repo-folder>
   ```

2. **Set Up a Virtual Environment (Recommended)**:  
   Create and activate a virtual environment:  
   ```bash
   python3 -m venv venv && source venv/bin/activate
   ```  
   Install the required dependencies:  
   ```bash
   pip install -r requirements.txt
   ```

   For more information on managing virtual environments, refer to [this guide](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html).

3. **Manually Install Key Libraries (If Needed)**:    
   ```bash
   pip install pandas numpy matplotlib seaborn scipy
   ```

## **Running the Jupyter Notebook**  
1. Clone the repository and save the folder.  
2. Open **Jupyter Notebook** from the command line or start menu:  
3. Navigate to the saved project folder.  
4. Open **`Gender_Differences_in_Dietary_Intake.ipynb`**.  
5. In the Jupyter menu, click on `Cell` > `Run All` to execute the analysis.  

---

### **Required Libraries**

The following libraries are used in this project:

- **pandas**: For data manipulation.
- **numpy**: For numerical operations.
- **matplotlib**: For visualizations.
- **seaborn**: For statistical graphics.
- **scipy**: For statistical tests.


---

### **Conclusion:**

Gender plays a significant role in dietary intake, with males consuming more calories, protein, carbohydrates, and fats compared to females. The differences observed are statistically significant, indicating that they are unlikely to be due to random chance.

These findings suggest that gender should be considered when designing nutrition programs or public health policies. However, this analysis only shows a relationship, not causation, and other factors may also influence dietary habits.




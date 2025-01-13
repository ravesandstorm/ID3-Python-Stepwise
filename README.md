# ID3-Python-Stepwise

### Project Description: ID3 Algorithm Implementation in Python

This project implements the **ID3 (Iterative Dichotomiser 3)** algorithm in Python for decision tree learning. The algorithm uses entropy and information gain as metrics to build a decision tree from a dataset. This implementation provides step-by-step calculation of the entropy and information gain for better verification and understanding.

---

#### Major Steps:
1. **Input Data:** The script takes a string input for column names and data rows.
2. **Preprocessing:** The data is parsed into a DataFrame for easy manipulation and processing.
3. **Entropy Calculation:** 
   - Calculates the overall entropy of the target variable.
   - Calculates conditional entropy for each unique value of the input attributes.
4. **Information Gain:** 
   - Uses the entropy values to calculate the information gain for each attribute.
   - Outputs the formulas and intermediate steps for transparency.
5. **Decision Tree Logic:** The attribute with the highest information gain is selected for the split.

---

#### How to Use:
1. Clone this repository:
   ```bash
   git clone https://github.com/ravesandstorm/ID3-Python-Stepwise.git
   ```
2. Open the script in your Python environment.
3. Modify the `columns` and `data` variables to input your dataset.
4. Run the script to view entropy and information gain calculations for all the data.

---

#### Example:
Given the following dataset:

| Weather | Parents  | Cash | Exam | Decision  |
|---------|----------|------|------|-----------|
| sunny   | visit    | rich | yes  | cinema    |
| windy   | no-visit | rich | no   | shopping  |

The script calculates:
- Entropy of the dataset
- Conditional entropy for each attribute
- Information gain for each attribute

Sample output:
```
Entropy of Data = 0.9852 =   -(6/11)*log(6/11) - (5/11)*log(5/11)
Entropy for 'sunny' = 0.9183 =   -(4/6)*log(4/6) - (2/6)*log(2/6)
...
Info. Gain for 'Weather' = 0.1934 =  0.985 - [(6/11)*0.9183 + (5/11)*0.7222]
```

---

#### Dependencies:
- Python 3.8+
- Pandas
- NumPy
- Python Math library

---

Feel free to contribute, report issues, or suggest improvements! 😊

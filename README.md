# Part 4 – Data Visualization & Machine Learning

This folder contains my work for **Part 4** of the Python assignment, focusing on data analysis, plotting with Matplotlib/Seaborn, and a simple machine learning model.

## Files

- `part4_visualization_ml.ipynb`  
  Jupyter notebook with all code, plots, and outputs for Tasks 1–4.
- `students.csv`  
  Provided dataset of student exam scores and pass/fail outcome.
- `README.md`  
  This description file.

The notebook also generates the following plot images in this folder:

- `plot1_bar.png` – Bar chart of average score per subject (Matplotlib).
- `plot2_histogram.png` – Histogram of `avg_score`.
- `plot3_scatter.png` – Scatter plot of Math vs Science scores.
- `plot4_box.png` – Box plot of `avg_score` by pass/fail.
- `plot5_line.png` – Line chart of student index vs `avg_score`.
- `plot6_seaborn_bar.png` – Seaborn bar plot of average subject scores.
- `plot7_seaborn_scatter.png` – Seaborn scatter plot of Math vs Science colored by pass/fail.

## What the notebook does

1. **Task 1 – Data exploration**  
   - Loads `students.csv` into a pandas DataFrame.  
   - Shows shape, dtypes, and summary statistics.  
   - Counts passed vs failed students.  
   - Computes average subject scores for pass vs fail groups.  
   - Finds the student with the highest overall average across five subjects.

2. **Task 2 – Matplotlib visualizations**  
   - Creates an `avg_score` column for each student.  
   - Builds five Matplotlib plots (bar, histogram, scatter, box, line) and saves them as PNGs.

3. **Task 3 – Seaborn visualizations**  
   - Repeats the subject-mean bar plot using seaborn styling.  
   - Plots a scatter of Math vs Science scores coloured by pass/fail using `hue`.

4. **Task 4 – Machine learning model**  
   - Uses the five subject scores as features to predict `passed`.  
   - Splits data into train/test sets with `train_test_split`.  
   - Scales features using `StandardScaler`.  
   - Trains a `LogisticRegression` model and reports test accuracy.  
   - Prints model coefficients to see which subjects have the strongest influence on passing.

## How to run

1. Ensure Python and the required libraries are installed:

   ```bash
   py -m pip install pandas matplotlib seaborn scikit-learn
   ```

2. Open `part4_visualization_ml.ipynb` in VS Code (or Jupyter).  
3. Run **Kernel → Restart & Run All** so that all cells execute in order and all plots and metrics are visible in the saved notebook.
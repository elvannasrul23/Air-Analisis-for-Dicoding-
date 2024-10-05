Here is the updated README file that includes the instructions for cleaning the data, setting up the analysis, and running the dashboard. The cleaned data will be saved in the `dashboard` folder as per your request:

---

# Air Quality Analysis and Dashboard Project

## Project Overview
This project involves analyzing air quality data from three stations (Guanyuan, Aotizhongxin, Tiantan) using Python, followed by creating a Streamlit-based dashboard to visualize the analysis results.

## Steps to Run the Project

### 1. Setup Environment
Begin by opening Anaconda PowerShell Prompt or a terminal. Then activate your environment, create the project directory, and install the necessary libraries.

```bash
# Activate the conda environment
conda activate main-ds

# Create a directory for the project
mkdir air_analisis

# Navigate into the directory
cd air_analisis

# Install the necessary libraries
pip install numpy pandas scipy matplotlib seaborn jupyter
```

### 2. Set Up Data and Code Files
#### 2.1 Data Folder
Inside the `air_analisis` directory, create a folder named `Data` where you will place the original CSV files containing the raw data.

```bash
# Create Data folder
mkdir Data
```

Place the following 3 CSV files in the `Data` folder:
- `PRSA_Data_Guanyuan_20130301-20170228.csv`
- `PRSA_Data_Aotizhongxin_20130301-20170228.csv`
- `PRSA_Data_Tiantan_20130301-20170228.csv`

#### 2.2 Dashboard Folder
Create another folder named `dashboard` where you will store the cleaned data and the Streamlit dashboard code.

```bash
# Create dashboard folder
mkdir dashboard
```

This folder will contain:
- The cleaned versions of the CSV files saved by your analysis notebook.
- The `dashboard.py` file, which contains the code for the Streamlit dashboard.

### 3. Jupyter Notebook Analysis

Start Jupyter Notebook to run the data analysis process:

```bash
jupyter-notebook
```

Create a new file named `notebook.ipynb` inside the `air_analisis` folder. This notebook will contain the code to load the raw data, clean it, and perform analysis (e.g., calculating PM2.5 trends, correlations, seasonal variations).

Once the analysis is complete, save the cleaned CSV files in the `dashboard` folder with the following names:
- `cleaned_guanyuan.csv`
- `cleaned_aotizhongxin.csv`
- `cleaned_tiantan.csv`

The notebook will handle the data cleaning and save these cleaned files automatically.

### 4. Running the Dashboard

To run the dashboard, first, install Streamlit if you haven't already:

```bash
pip install streamlit
```

Now, navigate to the `dashboard` folder and run the dashboard:

```bash
cd dashboard
streamlit run dashboard.py
```

### 5. Files Structure

After completing the above steps, your folder structure should look like this:

```bash
air_analisis/
│
├── Data/
│   ├── PRSA_Data_Guanyuan_20130301-20170228.csv
│   ├── PRSA_Data_Aotizhongxin_20130301-20170228.csv
│   └── PRSA_Data_Tiantan_20130301-20170228.csv
│
├── dashboard/
│   ├── cleaned_guanyuan.csv
│   ├── cleaned_aotizhongxin.csv
│   ├── cleaned_tiantan.csv
│   └── dashboard.py
│
└── notebook.ipynb
```

---

This README now includes steps for setting up the project, cleaning the data, and running the dashboard with Streamlit.

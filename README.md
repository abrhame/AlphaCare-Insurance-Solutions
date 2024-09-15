# AlphaCare Insurance Solutions

Welcome to the AlphaCare Insurance Solutions repository! This project focuses on analyzing historical insurance claim data to optimize marketing strategies and discover low-risk targets for premium adjustments.

## Project Overview

This repository contains code and documentation for data analysis and version control tasks performed for AlphaCare Insurance Solutions.

### Task 1: Exploratory Data Analysis (EDA) & Statistics

#### Objectives

- Perform Exploratory Data Analysis (EDA) on historical insurance claim data.
- Generate insights through statistical analysis and visualization.
- Provide actionable recommendations based on the analysis.

#### Key Tasks

1. **Data Summarization**:
   - Descriptive statistics for numerical features.
   - Review data types and formats.
   
2. **Data Quality Assessment**:
   - Check for missing values.
   
3. **Univariate Analysis**:
   - Plot histograms for numerical columns and bar charts for categorical columns.
   
4. **Bivariate/Multivariate Analysis**:
   - Explore relationships between features using scatter plots and correlation matrices.
   
5. **Data Comparison**:
   - Analyze trends and changes across geographic regions.
   
6. **Outlier Detection**:
   - Use box plots to identify outliers.

7. **Visualization**:
   - Create at least three insightful plots from the EDA.

### Task 2: Data Version Control (DVC)

#### Objectives

- Implement Data Version Control (DVC) to manage large datasets effectively.
- Set up local remote storage for tracking data versions.
- Integrate DVC with Git to manage data alongside code.

#### Key Tasks

1. **Install DVC**:
   - Install DVC in the Python environment using `pip install dvc`.
   
2. **Initialize DVC**:
   - Run `dvc init` to initialize DVC in the project directory.
   
3. **Set Up Local Remote Storage**:
   - Create a directory for local storage.
   - Configure the storage as a DVC remote using `dvc remote add -d localstorage /path/to/storage`.
   
4. **Add and Track Data**:
   - Use `dvc add <data.csv>` to add data files to DVC.
   
5. **Commit Changes**:
   - Commit the `.dvc` files to Git to track data versions.
   
6. **Push Data to Remote**:
   - Use `dvc push` to upload data to the configured remote storage.

## Getting Started

1. Clone the repository:

    ```bash
    git clone https://github.com/abrhame/AlphaCare-Insurance-Solutions.git
    cd AlphaCare-Insurance-Solutions
    ```

2. Set up a Python virtual environment and install dependencies:

    ```bash
    python -m venv venv
    source venv/bin/activate
    pip install -r requirements.txt
    ```

3. Initialize and configure DVC:

    ```bash
    dvc init
    dvc remote add -d localstorage /path/to/storage
    ```

4. Add and track your data with DVC:

    ```bash
    dvc add data/MachineLearningRating_v3.txt
    git add data/MachineLearningRating_v3.txt.dvc .gitignore
    git commit -m "Add dataset to DVC"
    dvc push
    ```

## Contributing

Feel free to contribute to this project by submitting issues or pull requests.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

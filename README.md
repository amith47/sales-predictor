# Sales Predictor

This project forecasts future sales for a specific item in a specific store using historical sales data. It uses time series analysis and compares ARIMA and SARIMAX models to select the best forecasting approach.

## Dataset
The dataset is located at `data/train.csv` and contains the following columns:
- `date`: Date of the sale
- `store`: Store ID
- `item`: Item ID
- `sales`: Number of items sold at a particular store on a particular date

## Project Structure
- `sales_forecasting.ipynb`: Jupyter notebook with all analysis, modeling, and forecasting steps
- `data/train.csv`: Historical sales data

## How to Run the Project

### 1. Set Up the Environment
1. Ensure you have Python 3.8+ installed.
2. (Recommended) Create a virtual environment:
   ```sh
   python -m venv .venv
   .venv\Scripts\activate  # On Windows
   # or
   source .venv/bin/activate  # On Mac/Linux
   ```
3. Install required packages:
   ```sh
   pip install jupyter pandas numpy matplotlib seaborn statsmodels scikit-learn
   ```

### 2. Start Jupyter Notebook
1. In the project directory, run:
   ```sh
   jupyter notebook
   ```
2. Open `sales_forecasting.ipynb` in your browser.

### 3. Execute the Notebook
1. Run all cells in order (from top to bottom) for a complete workflow:
   - Data loading and inspection
   - Filtering for a specific store and item
   - Exploratory Data Analysis (EDA)
   - Stationarity checks
   - Train-test split
   - ARIMA and SARIMAX modeling
   - Model evaluation and comparison
   - Forecasting future sales
2. You can change the `store_id` and `item_id` variables in the notebook to forecast for different store-item pairs.

## Notes
- Make sure to run all cells in order to avoid variable errors.
- The notebook will guide you through each step and display results and plots.

## License
This project is for educational and demonstration purposes.

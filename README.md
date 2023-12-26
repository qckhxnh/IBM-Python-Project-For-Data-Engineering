# ETL Practice Project

This repository contains a simple ETL (Extract, Transform, Load) script named `main.py` that processes data from CSV, JSON, and XML files. The script downloads data from a provided link, extracts information, transforms the 'price' values, and loads the transformed data into a CSV file. The ETL process is logged at different stages to track progress.

## Project Structure

- `data_source`: Folder to store the downloaded and extracted data files.
- `main.py`: Python script implementing the ETL pipeline.
- `log_file.txt`: Log file recording the progress of the ETL process.
- `transformed_data.csv`: CSV file where the transformed data is loaded.

## How to Use

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/your-username/etl-practice.git
   cd etl-practice
   ```

2. **Download and Unzip Data:**
   ```bash
   mkdir data_source
   cd data_source
   wget https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-PY0221EN-SkillsNetwork/labs/module%206/Lab%20-%20Extract%20Transform%20Load/data/datasource.zip
   unzip datasource.zip
   ```

3. **Install Dependencies:**
   Ensure you have Python installed. Install the required packages using:
   ```bash
   pip install pandas
   ```

4. **Run the ETL Pipeline:**
   Execute the ETL pipeline script:
   ```bash
   python etl_practice.py
   ```

5. **Check the Output:**
   The transformed data will be saved in `transformed_data.csv`, and the progress will be logged in `log_file.txt`.

## ETL Process Steps

1. **Extraction:**
   - Data is extracted from CSV, JSON, and XML files in the `data_source` folder.
   - The headers are 'car_model', 'year_of_manufacture', 'price', and 'fuel'.

2. **Transformation:**
   - The 'price' values are rounded to two decimal places.

3. **Loading:**
   - Transformed data is loaded into the `transformed_data.csv` file.

4. **Logging:**
   - Timestamped logs are recorded in `log_file.txt` at different ETL process stages.

## Logs

Review the `log_file.txt` for detailed information on the progress of each phase in the ETL process.

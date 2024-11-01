# CSV_analyzer_web3
# CSV Analyzer and Report Generating App

This web application allows users to upload CSV files and automatically generate comprehensive exploratory data analysis reports using ydata-profiling (formerly pandas-profiling).

## Prerequisites

- Google Colab or VS Code
- Python 3.x
- Internet connection
- Ngrok account and authentication token

## Required Libraries

```python
streamlit
pandas
ydata-profiling
streamlit-pandas-profiling
pyngrok
```

## Setup and Installation

1. **Download the Project**
   - Download the provided `.ipynb` notebook file
   - Open it in Google Colab (recommended) or VS Code
     (NOTE: I have used colab as my VScode was facing some technical issue)

2. **Install Required Libraries**
   - Run the installation cells in the notebook
   - Make sure all required libraries are properly installed

3. **Configure Ngrok**
   - Sign up for a free account at [ngrok.com](https://ngrok.com)
   - Get your authentication token from the ngrok dashboard
   - Replace "HERE_AUTH_TOKEN" in the code with your personal ngrok authentication token
     ![image](https://github.com/user-attachments/assets/92b61426-603c-4f16-a70a-764d58938798)


## Running the Application

1. **Execute the Code**
   - Run all cells in the notebook sequentially
   - After the app.py code is run it creates a file in the contents of local storage
     ![image](https://github.com/user-attachments/assets/dbbd912c-4af5-4f97-9e23-092ef127ddc9)

   - Wait for the Streamlit application to initialize

2. **Access the Web Interface**
   - After running the app, an ngrok URL will be generated
   - Click on the provided ngrok link (format: `https://xxxx-xx-xxx-xxx-xx.ngrok-free.app`)
     
     ![image](https://github.com/user-attachments/assets/6e7902da-59c6-4bce-9ef5-5a8bac07f02b)
     
   - You'll see a security warning from ngrok - click "Visit Site"
     ![image](https://github.com/user-attachments/assets/d526f608-6502-48c7-9291-ddaa602d9644)


3. **Using the Web Interface**
   - The main page will show "Exploratory Data Analysis (EDA) App"
     ![image](https://github.com/user-attachments/assets/e9ef4682-9103-4035-9fba-e21f1e9a70d9)

   - Click on "Browse files" to select and upload your CSV file
   - The app accepts only CSV file formats
   - After uploading, a data preview will be shown

4. **Generating and Viewing Reports**
   - The application will automatically generate a detailed EDA report
   - Processing time varies depending on the size of your CSV file
   - The report will include:
     - Data overview
     - Variable analysis
     - Correlations
     - Missing values
     - Statistical information

     ![image](https://github.com/user-attachments/assets/769f96eb-29a6-4f10-8e98-da2142aa4cc1)


5. **Downloading Reports**
   - Once the report is generated, you can view it directly in the browser
   - Use the "Download Report" button to save the report as an HTML file
   - Downloaded reports can be viewed offline in any web browser

     ![image](https://github.com/user-attachments/assets/e2c99ac4-896a-4880-b79e-6a5aefe0627f)


## Important Notes

- The application uses ISO-8859-1 encoding for reading some kind of CSV files which has encoding
- Large CSV files may take longer to process
- The ngrok URL is temporary and will change each time you run the application
- Make sure to keep your ngrok authentication token private

## Troubleshooting

- If the application doesn't load, check your internet connection
- Ensure all required libraries are properly installed
- Verify that your ngrok authentication token is correct
- If using VS Code, make sure you have the necessary extensions installed

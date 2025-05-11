```
Name : Subikshan P
Reg.No : 212223240161
```
# RPA_Ex-05
# Aim:
  To create a UiPath workflow that scrapes structured data from a website and saves it into a CSV file.

# Materials Required:
UiPath Studio (Community or Enterprise Edition) Internet connection A sample website to scrape (e.g., https://www.amazon.com) Basic knowledge of UiPath's Data Scraping Wizard
# PROCEDURE:

## Step 1:
Create a New Process Open UiPath Studio and create a new process named WebScrapingExample.

## Step 2: 
Open the Target Website Open your web browser and go to: [https://www.amazon.com] Step 3: Use Data Scraping Wizard In UiPath Studio, click on "Data Scraping" from the Design tab.
Save this file in your project directory.
When the wizard opens:
Click on the first product title.

## Step 3: 
Then click on the second product title to teach the pattern.

When prompted, extract URL as well (optional).

Click Next, then Finish.

The extracted data will be stored in a DataTable variable (e.g., ExtractDataTable).

## Step 4: 
 Write Data to CSV After the Data Scraping activity, drag a Write CSV activity.

Properties: Input: ExtractDataTable FilePath: "BooksData.csv" (you can choose your own name) Include Headers: ✔️ (checked)

## Step 5:
Add Second Excel Application Scope Below the first scope, drag another Excel Application Scope.
Set the path to "Output.xlsx" (can be a new empty file).

## Step 6: 
Run the Workflow

Save the workflow. Click Run.

# Output:

![5-1](https://github.com/user-attachments/assets/c477f5d1-7962-482c-a7d7-cd088b39f5ca)

A CSV file named BooksData.csv will be created in your project folder with data like:
![5-2](https://github.com/user-attachments/assets/a6b6325e-8580-4cb7-8a38-a1c19cff11a0)


## Result:
The workflow successfully scrapes data from the website and saves it into a CSV file using UiPath's Data Scraping and File I/O activities.

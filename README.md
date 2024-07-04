# Expense Tracking System

## Objective
Develop a system to track expenses and provide analytics to identify trends, drivers, and insights.

## Description
The Expense Tracking System is designed to streamline expense logging and analysis. Users can log expenses through a user-friendly interface and visualize spending patterns using interactive dashboards.

## Features
- **Expense Logging**: Easily log expenses through a designated interface.
- **Data Visualization**: Visualize expense data using tools like Power BI, Excel, or Google Sheets.
- **Trend Analysis**: Analyze spending trends over time to identify patterns and outliers.
- **Driver Identification**: Identify key drivers of expenses to prioritize cost-saving opportunities.
- **Actionable Insights**: Generate actionable insights for improved financial planning and decision-making.

## Code Snippet (Google Apps Script)
```javascript
/** @OnlyCurrentDoc */

function Adjust_Formatting() {
  var spreadsheet = SpreadsheetApp.getActive();
  var sheet = spreadsheet.getActiveSheet();
  sheet.getRange(1, 1, sheet.getMaxRows(), sheet.getMaxColumns()).activate();
  spreadsheet.getRange('2:2').copyTo(spreadsheet.getActiveRange(), SpreadsheetApp.CopyPasteType.PASTE_FORMAT, false);
  spreadsheet.getRange('A1').activate();
};

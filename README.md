# Apex Data Type Mapper

A modern, browser-based tool that allows Salesforce developers and admins to **generate Apex upsert scripts** from **tabular data** like CSV, TSV, or spreadsheet exports. Built using vanilla JavaScript and styled with TailwindCSS.


## Features

* Parse tabular data (CSV, TSV, etc.)
* Auto-infer Apex data types (`String`, `Boolean`, `Date`, etc.)
* Manual override for data type mapping
* Smart detection of unique identifier field (e.g. `Name`)
* Generate downloadable `.cls` Apex class files for each record
* All in-browser, no backend required


## No Data Leaves Your Browser

This tool is entirely front-end based. No data is sent to any server. You can use it safely in secure environments or locally without internet access.

## Quick Start

1. **Open the HTML file** in any modern browser (Chrome, Edge, Firefox).
2. Enter:

   * `sObject Record Name` (e.g., `MyObject__c`)
   * The tabular **data** with headers (e.g., copy from Excel or Google Sheets)
   * Select the appropriate **separator** (comma, tab, semicolon, etc.)
   * Choose the **unique identifier column** (e.g., `Name`)
3. Click **"Parse Headers"**
4. Review and adjust data types if necessary
5. Click **"Generate Apex Scripts"** to download `.cls` files for each record


## Data Format

Ensure your input data has:

* A **header row** (first row = field names)
* Consistent separators (`,`, tab, `;`, etc.)
* A **unique identifier column** (e.g., `Name` or `External_ID__c`)

### Example Input:

```
fifty,new,my,till,expect,Name
compass,characteristic,distance,said,who,cloud
rope,present,tape,begun,death,hospital
```

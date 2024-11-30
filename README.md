# Multi-Task Robots Project 🤖

This project contains three distinct automation robots, built with **UiPath**, designed to perform specific tasks efficiently. These robots streamline data handling, form submissions, and duplicate-checking processes, showcasing the power of automation.

---

## 🚀 Robots Overview

### 🤖 **Robot 1: Excel Data Copier**
- **File**: `Robot1.xaml`
- **Purpose**: Merges data from multiple Excel files into a single unified sheet.
- **Workflow**:
  1. Reads data from `cars1.xlsx`, `cars2.xlsx`, and `cars3.xlsx`.
  2. Aligns all data under the column structure of `cars1.xlsx`.
  3. Saves the consolidated data into `newcar.xlsx`.

---

### 🤖 **Robot 2: Microsoft Form Automation**
- **File**: `Robot2.xaml`
- **Purpose**: Automates submission of raw data into a Microsoft Form.
- **Workflow**:
  1. Reads raw data from `cars.xlsx`.
  2. Inputs the data into a pre-configured Microsoft Form.
  3. Presses "Submit" for each record.

---

### 🤖 **Robot 3: Smart Microsoft Form Submission**
- **File**: `Robot4.xaml`
- **Purpose**: Submits unique data to a Microsoft Form, ensuring no duplicate submissions.
- **Workflow**:
  1. Reads raw data from `cars.xlsx`.
  2. Inputs the data into the Microsoft Form.
  3. Inputs "1" in the **value-added** field.
  4. Skips any previously submitted data.
  5. Submits the form for unique records only.

---

## 🛠️ Technologies Used
- **Automation Tool**: UiPath
- **Languages**: Visual workflows in UiPath
- **File Formats**:
  - Input: `.xlsx` (Excel)
  - Output: `.xlsx` (Excel)
- **Microsoft Form**: Web-based form integration for data submission

---
## 💻 Getting Started

### Prerequisites
- **UiPath Studio**: Install [UiPath Studio](https://www.uipath.com/) on your system.
- **Excel Application**: Ensure Microsoft Excel is installed to process `.xlsx` files.
- **Microsoft Form**: Create or access the form and retrieve its URL for use in the workflows.

---

### Running the Robots

#### 🤖 Robot 1: Excel Data Copier
1. Open `Robot1.xaml` in UiPath Studio.
2. Place the following files in the same directory as the project:
   - `cars1.xlsx`
   - `cars2.xlsx`
   - `cars3.xlsx`
3. Run the workflow.
4. The merged file will be saved as `newcar.xlsx`.

#### 🤖 Robot 2: Microsoft Form Automation
1. Open `Robot2.xaml` in UiPath Studio.
2. Place `cars.xlsx` in the same directory as the project.
3. Update the form URL in the workflow to match your Microsoft Form link.
4. Run the workflow to automate data submission.

#### 🤖 Robot 3: Smart Microsoft Form Submission
1. Open `Robot4.xaml` in UiPath Studio.
2. Place `cars.xlsx` in the same directory as the project.
3. Update the form URL in the workflow to match your Microsoft Form link.
4. Run the workflow:
   - The robot will submit only unique records.
   - It will input "1" in the **value-added** field before submission.

---
```plaintext
robots-project/
├── .local/                # Local UiPath configuration files
├── .objects/              # UiPath object files
├── .project/              # UiPath project metadata
├── .screenshots/          # Screenshots for documentation (if applicable)
├── .settings/             # UiPath project settings
├── .tmh/                  # Temp metadata for UiPath project
├── cars.xlsx              # Source raw data file
├── cars1.xlsx             # Input file for Robot 1
├── cars2.xlsx             # Input file for Robot 1
├── cars3.xlsx             # Input file for Robot 1
├── newcar.xlsx            # Output file created by Robot 1
├── Robot1.xaml            # UiPath workflow for Robot 1
├── Robot2.xaml            # UiPath workflow for Robot 2
├── Robot4.xaml            # UiPath workflow for Robot 3
├── Main.xaml.json         # UiPath project metadata
├── project.json           # UiPath project configuration
└── README.md              # Project documentation



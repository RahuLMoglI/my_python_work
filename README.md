# my_python_work
This Python script is designed to automate the process of analyzing log files and generating an organized Excel report for simulation or regression testing. Here's an overview of its functionality:

Key Features:
Error Signature Parsing: The script extracts error signatures from an input_error.log file using regular expressions and stores them in variables.
Log File Traversal: It searches through directories for log files and identifies simulation test cases by matching folder names and logs with specific error patterns.
Error Detection: The script identifies and categorizes various types of errors, including:
Compilation errors
Boot errors
Hung cases
Test failures
Excel Report Generation: It creates an Excel report with detailed information about error occurrences. The report is structured into multiple sheets, including:
Detailed report: Organized error messages and counts.
Regression status: Counts of different error types (e.g., compilation errors, boot errors).
First Error Logs: For failed tests, boot errors, and hung cases.
Directory Management: The script dynamically generates directories for saving the output based on the current date and time.
User Inputs: It accepts inputs such as the path to the regression directory and allows for defaulting to the current directory.
Temporary Files Cleanup: Temporary files created during execution are deleted after completion.
Usage:
The user runs the script, provides the required inputs, and receives an organized Excel report containing error details and summary statistics.
The Excel file is saved in a structured directory (excel_reports/<Year>/<Month>/<Day>/).
This script is ideal for anyone who wants to automate the task of analyzing simulation logs and generating error reports, especially in a verification or regression testing environment.

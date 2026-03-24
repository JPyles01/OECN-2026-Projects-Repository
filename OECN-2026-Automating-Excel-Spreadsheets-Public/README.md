# OECN 2026 Automating Excel Spreadsheets
This repo contains project examples from the Automating Excel Spreadsheets with Python session at OECN United 2026.

Project 1: Password Reminder Project - Easy:
This project looks through all districts in the input folder and looks for a USAS User Report.csv file and a USPS User Report.csv file. The file names do matter. It determines which application to write to the output file based on the application within the file name. The reports used to create these files are in the SSDT report json files in the Password Reminder Project - Easy folder. There are two files. One for the USAS application and one for the USPS application. These reports pull information from the Users grid in USAS and USPS.
This project writes the user information to a master "user_listings.csv" file in the output folder. It also writes the district and application for the user.


Project 2: Financial Graphs Project - Hard:
This project looks through each district in the input folder for 3 reports. The reports are called Graphs - Cash Account History, Graphs - Expenditures Pie Chart, and Graphs - Revenue Pie Chart. The json files for these reports are in the SSDT report json files folder. The program uses the input district folder's name to determine what district it is currently working in. The program reads through these input files, formats it, and writes it to a graphs.xlsx file in the output folder. It puts the district name in the file name. If multiple cash accounts are in the input file, it makes a file for each account.

The pie charts may encounter errors depending on the district's input files. The pie charts categorieses the slices by object levels and receipt levels. Some districts account codes can be different. For example, ESCs categories may look very different compared to a normal school district. There is error handling to catch errors.


Project 3: AI Prompt Example:
This is a demonstration of what google gemini can produce. All it does it reads one row in an input file and writes it to an output file. It writes to the next available month in the output file.



Note about config files:
All file paths can be defined in the config.ini files.

Note about emails:
By default, emailing will not work. They were removed so this could publicaly be posted on git hub. The config files must be updated with proper email addresses, host numbers, port numbers, and server names.
If the sending email address has a password, the code must be edited to use a password from the config.ini files.


The 2 projects contain a requirements.txt file which list the python libraries necessary for the project. Python has a command that can read this txt file and download the same libraries.

Projects were created by Jon Pyles at NOACSC.


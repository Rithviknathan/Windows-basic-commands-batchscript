# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

# AIM:
To execute Windows basic commands and batch scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2:

Write the Windows commands / batch file
Save each script in a file with a .bat extension.
Ensure you have the necessary permissions to perform the operations.
Adapt paths as needed based on your system configuration.
### Step 3:

Execute the necessary commands/batch file for the desired output. 




# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "MyLab" on the desktop.


## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\MyLab
```
![ex8op1](https://github.com/Rithviknathan/Windows-basic-commands-batchscript/assets/148410509/983b92c5-927e-4594-bb9c-414eafbd5388)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
```
cd %userprofile%\Desktop\MyLab
```
![ex8op2](https://github.com/Rithviknathan/Windows-basic-commands-batchscript/assets/148410509/62cd5c3c-b3e9-4718-92f0-c9c4b3c5afe7)
```
type nul > MyFile.txt
```
![ex8op3](https://github.com/Rithviknathan/Windows-basic-commands-batchscript/assets/148410509/567f6dd8-1dca-4a1f-8b73-b8dbc412c15a)
List the contents of the "MyLab" directory.
## COMMAND AND OUTPUT
```
dir %userprofile%\Desktop\MyLab
```
![ex8op4](https://github.com/Rithviknathan/Windows-basic-commands-batchscript/assets/148410509/1b050a53-f233-4122-9f6c-c384a3c16a4b)
Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Backup
```
![ex8op5](https://github.com/Rithviknathan/Windows-basic-commands-batchscript/assets/148410509/643757f7-cfd7-4157-91b7-18d666d816b9)
```
copy MyFile.txt %userprofile%\Desktop\Backup
```
![ex8op6](https://github.com/Rithviknathan/Windows-basic-commands-batchscript/assets/148410509/c93b410f-81e1-47b2-9a1d-d7075ec12067)
Move the "MyLab" directory to the "Documents" folder.
## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Documents
```
![ex8op7](https://github.com/Rithviknathan/Windows-basic-commands-batchscript/assets/148410509/bdfe8c59-5ddb-422c-bf91-97ee1d72087e)
move MyLab Documents

## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
## COMMAND:
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
## OUTPUT
![ex8op8](https://github.com/Rithviknathan/Windows-basic-commands-batchscript/assets/148410509/21b870bf-e1a9-4ca9-87ed-6eea5c7e2fb8)
## COMMAND:
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```
## OUTPUT
![ex8op9](https://github.com/Rithviknathan/Windows-basic-commands-batchscript/assets/148410509/64c6818f-f8c5-4e8e-9bb4-6f59f2ec4d29)

# RESULT:
The commands/batch files are executed successfully.


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
mkdir %userprofile%\Desktop\MyLab
![ex8op1](https://github.com/user-attachments/assets/2ca83fdc-ca5c-4443-8833-474de589bdd2)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab
![ex8op2](https://github.com/user-attachments/assets/ca50a4dc-10dc-477f-a64c-fa68bb3d6a73)
type nul > MyFile.txt
![ex8op3](https://github.com/user-attachments/assets/b8a31a20-e740-438c-beac-6444f8492e49)

List the contents of the "MyLab" directory.

## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLab
![ex8op4](https://github.com/user-attachments/assets/bfc760fd-8753-492f-b675-8e714de170e8)


Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\Backup
![ex8op5](https://github.com/user-attachments/assets/e4d93ae6-2f94-4a23-9e8a-0173f56f5a9f)
copy MyFile.txt %userprofile%\Desktop\Backup
![ex8op6](https://github.com/user-attachments/assets/05ff7735-ac64-419b-953c-f48e63d75e31)

Move the "MyLab" directory to the "Documents" folder.

## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\Documents

move MyLab Documents
![ex8op7](https://github.com/user-attachments/assets/822bc06d-e843-44db-aaea-7bfee500b9cc)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

## COMMAND:
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!

## OUTPUT
![ex8op8](https://github.com/user-attachments/assets/fef3decc-f12a-4a40-86a5-7d1591421b1b)

## COMMAND:
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!

## OUTPUT:
![ex8op9](https://github.com/user-attachments/assets/d063ef09-757a-4eea-bd9b-916b1a130b63)


## RESULT:
The commands/batch files are executed successfully.


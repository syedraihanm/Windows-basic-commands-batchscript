## Name: Syed Mohamed Raihan M
## Regno: 212224240144

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


![image](https://github.com/Priyanghaofficial/Windows-basic-commands-batchscript/assets/147121154/f874ddb1-ee02-4a98-866c-822976c70384)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab


![image](https://github.com/Priyanghaofficial/Windows-basic-commands-batchscript/assets/147121154/0998bd8b-6891-47cf-9be5-8d3fe2c6ddb8)
![image](https://github.com/Priyanghaofficial/Windows-basic-commands-batchscript/assets/147121154/2ba4c6bb-8c38-4ce0-9527-af157449dc1a)

List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLab


![image](https://github.com/Priyanghaofficial/Windows-basic-commands-batchscript/assets/147121154/81982adb-dd79-4df5-bf38-6e577ff4c630)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup


![image](https://github.com/Priyanghaofficial/Windows-basic-commands-batchscript/assets/147121154/88f01d4b-df99-49b1-84a9-c566a7c4aa11)
![image](https://github.com/Priyanghaofficial/Windows-basic-commands-batchscript/assets/147121154/f6e9c1c3-ec06-4cc1-a394-63bd6f2c25c9)

Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
mv Myfile.txt %userprofile%\Documents

![image](https://github.com/Priyanghaofficial/Windows-basic-commands-batchscript/assets/147121154/05a6d26d-62b1-47d9-91de-53c37f29ee72)

## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!

Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup.


@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!




## OUTPUT
![image](https://github.com/Priyanghaofficial/Windows-basic-commands-batchscript/assets/147121154/937daaff-887f-400b-a7f6-81ed1783397c)






# RESULT:
The commands/batch files are executed successfully.

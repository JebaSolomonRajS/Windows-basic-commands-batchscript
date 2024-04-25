# Windows-basic-commands-batchscript
## Ex08-Windows-basic-commands-batchscript

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
Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
```
mkdir %userprofile%\Desktop\MyLab
```
![image](https://github.com/JebaSolomonRajS/Windows-basic-commands-batchscript/assets/139432449/0c85347a-e9ff-4e6b-b7e3-9203796071ae)


## COMMAND AND OUTPUT
List the contents of the "MyLab" directory.
```
cd %userprofile%\Desktop\MyLab
```
![image](https://github.com/JebaSolomonRajS/Windows-basic-commands-batchscript/assets/139432449/481b6c6d-db2e-427a-8bd4-ebdd07e59ed0)

![image](https://github.com/JebaSolomonRajS/Windows-basic-commands-batchscript/assets/139432449/6df34d4d-3f78-40b7-b1c4-4f7e419c3c39)


## COMMAND AND OUTPUT
Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
dir %userprofile%\Desktop\MyLab
```
![image](https://github.com/JebaSolomonRajS/Windows-basic-commands-batchscript/assets/139432449/2ef8798d-99fe-4f2e-a719-4f143e29383c)


## COMMAND AND OUTPUT
Move the "MyLab" directory to the "Documents" folder.
```
mkdir %userprofile%\Desktop\Backup
copy MyFile.txt %userprofile%\Desktop\Backup
```
![image](https://github.com/JebaSolomonRajS/Windows-basic-commands-batchscript/assets/139432449/cf6323b5-3cc4-414a-81f4-a550aacb8dae)
![image](https://github.com/JebaSolomonRajS/Windows-basic-commands-batchscript/assets/139432449/73d10ff4-d9d7-4b7f-ad88-6f0bfb6eebfe)


## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```
![image](https://github.com/JebaSolomonRajS/Windows-basic-commands-batchscript/assets/139432449/2c8c31a2-0050-4f1a-8103-01c8a7e3f8d2)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```
## OUTPUT
![image](https://github.com/JebaSolomonRajS/Windows-basic-commands-batchscript/assets/139432449/dd22aee4-b2e1-4202-85c0-1addaeca663f)

# RESULT:
The commands/batch files are executed successfully.

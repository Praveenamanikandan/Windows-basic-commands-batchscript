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

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
```
mkdir %userprofile%\Desktop\MyLab
```
![image](https://github.com/Praveenamanikandan/Windows-basic-commands-batchscript/assets/144870776/2cff8114-5e4a-4cc7-a869-044402f6cb37)


## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```
cd %userprofile%\Desktop\MyLab
```
![image](https://github.com/Praveenamanikandan/Windows-basic-commands-batchscript/assets/144870776/9343298e-0913-4cde-b967-65b361cfdc83)
![image](https://github.com/Praveenamanikandan/Windows-basic-commands-batchscript/assets/144870776/007e3be0-0578-4b62-83b1-4f7317e8d508)


## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
dir %userprofile%\Desktop\MyLab
```
![image](https://github.com/Praveenamanikandan/Windows-basic-commands-batchscript/assets/144870776/7f2c2939-1cdb-483c-af72-c7fad3811149)

## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.
```
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
```
![image](https://github.com/Praveenamanikandan/Windows-basic-commands-batchscript/assets/144870776/0dfddcb2-4c0f-4052-b203-eea2f926714a)

## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```
![image](https://github.com/Praveenamanikandan/Windows-basic-commands-batchscript/assets/144870776/1f784ee5-4e1b-48e2-b366-85679e070775)

## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!


@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```
## OUTPUT



![image](https://github.com/Praveenamanikandan/Windows-basic-commands-batchscript/assets/144870776/fcf18b26-c17c-4d20-a8ac-f477fd9bc0cd)


# RESULT:
The commands/batch files are executed successfully.


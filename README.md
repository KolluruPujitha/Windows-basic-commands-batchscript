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

![image](https://github.com/KolluruPujitha/Windows-basic-commands-batchscript/assets/150231340/bcf05284-b71e-40fd-aaf4-8185eea27d23)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab

![image](https://github.com/KolluruPujitha/Windows-basic-commands-batchscript/assets/150231340/3667b371-6dbc-4b32-b368-cdcc64fd16cd)

![image](https://github.com/KolluruPujitha/Windows-basic-commands-batchscript/assets/150231340/ae32de33-c518-4ab7-b5fc-fd59b8acf835)

List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLab

![image](https://github.com/KolluruPujitha/Windows-basic-commands-batchscript/assets/150231340/89fcc231-ca79-4c09-b3fd-17568bcfdcdb)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
```


![image](https://github.com/KolluruPujitha/Windows-basic-commands-batchscript/assets/150231340/9401e952-45ca-415f-8d80-534a89824e40)
![image](https://github.com/KolluruPujitha/Windows-basic-commands-batchscript/assets/150231340/d9a41130-31da-4bcb-bcc8-8c522f6c7369)

Move the "MyLab" directory to the "Documents" folder.
## COMMAND AND OUTPUT
mv Myfile.txt %userprofile%\Documents

![image](https://github.com/KolluruPujitha/Windows-basic-commands-batchscript/assets/150231340/566f139f-cc26-4ce1-81f0-725b31b4434d)


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

![image](https://github.com/KolluruPujitha/Windows-basic-commands-batchscript/assets/150231340/1ee7d9b1-f0ad-4176-86ea-bf5193debbeb)


# RESULT:
The commands/batch files are executed successfully.


## NAME:PRIDEESH M
## REG NO:212223040154


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
![325488048-cb3eb77e-19eb-4685-8d73-f957d261233b](https://github.com/prideeshm/Windows-basic-commands-batchscript/assets/144870483/2bc1d816-c20d-4780-b52c-c410f0878aad)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
## COMMAND AND OUTPUT
```
cd %userprofile%\Desktop\MyLab
```
![325488125-4d29f61c-0e88-42cf-872e-b1ff09202912](https://github.com/prideeshm/Windows-basic-commands-batchscript/assets/144870483/4e31a8f3-cea7-4210-be0c-7e621f09823c)


![325488188-637c9afc-cecf-406f-a9ef-dcf61c75f411](https://github.com/prideeshm/Windows-basic-commands-batchscript/assets/144870483/11722917-9e16-4c9e-b237-b6b467172dbc)


List the contents of the "MyLab" directory.
## COMMAND AND OUTPUT
```
dir %userprofile%\Desktop\MyLab
```

![325488240-d4197033-9d04-4550-8513-0248fc20144c](https://github.com/prideeshm/Windows-basic-commands-batchscript/assets/144870483/6c55a3ac-3475-40a9-ad6d-45a05979c914)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
```
![325488328-8bc9e2ac-0919-477b-b025-39a945f7afb2](https://github.com/prideeshm/Windows-basic-commands-batchscript/assets/144870483/ed2c5e47-161b-450a-91aa-ddfb79809a9a)


![325488396-fefdde05-4d84-46ee-9135-d1d3c9b7e77c](https://github.com/prideeshm/Windows-basic-commands-batchscript/assets/144870483/32d51147-d85b-4e3b-8dbb-e1975510360c)


Move the "MyLab" directory to the "Documents" folder.

## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```

![325488484-2cfa13a1-6152-4f01-bbe4-4a310c0409a9](https://github.com/prideeshm/Windows-basic-commands-batchscript/assets/144870483/bf9a1ada-de78-414e-974f-c0490d10e565)


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
![325488538-4a712e59-e8ca-47c3-880d-670aa06d9450](https://github.com/prideeshm/Windows-basic-commands-batchscript/assets/144870483/9e40847b-f7b6-4a33-94b3-2aafd5e310fe)


# RESULT:
The commands/batch files are executed successfully.


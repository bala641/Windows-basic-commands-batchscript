# NAME : BALA B
# REG NO : 212224100005
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

~~~bash
C:\Users\admin>mkdir Mylab
C:\Users\admin>cd Mylab
~~~
![image](https://github.com/user-attachments/assets/c88a8c66-5573-4d17-9703-7d1b2711854b)

## COMMAND AND OUTPUT
Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

~~~bash
C:\Users\admin\Mylab>echo > MyFile.txt
~~~
![image](https://github.com/user-attachments/assets/dc45ebae-a660-407d-8374-ed8a964b0ab3)

## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
~~~bash
C:\Users\admin\Mylab>dir
~~~
![image](https://github.com/user-attachments/assets/3cc0ec96-3f7a-4fd6-ac5a-5e4c5b76f886)

## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
~~~bash
copy "Mylab\MyFile.txt" "Backup\copy.txt"
~~~
![image](https://github.com/user-attachments/assets/0736563d-a3c1-4cb2-9de4-bafca42878f8)

## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.
~~~bash
move "Mylab\*.*" "Backup"
~~~
![image](https://github.com/user-attachments/assets/5a6b48e1-65ca-4f4a-b1ca-fff09b571fe4)

## COMMAND AND OUTPUT

## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

~~~bash
@echo off
REM BackupScript.bat - Copies all .docx files from Documents to Desktop\DocBackup

REM Define source and destination paths
set "source=%USERPROFILE%\C:\User\admin\Mylab"
set "destination=%USERPROFILE%\C:\User\admin\DocBackup"

REM Create the destination folder if it doesn't exist
if not exist "%destination%" (
    mkdir "%destination%"
)

REM Copy all .docx files
copy "%source%\*.docx" "%destination%"

echo Backup completed successfully.
pause

~~~


## OUTPUT

![image](https://github.com/user-attachments/assets/e0e9eb01-6811-4851-baae-f5dc38203978)




# RESULT:
The commands/batch files are executed successfully.


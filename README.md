[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/vbnbTt5m)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15279572&assignment_repo_type=AssignmentRepo)
# Dev_Setup
Setup Development Environment

#Assignment: Setting Up Your Developer Environment

#Objective:
This assignment aims to familiarize you with the tools and configurations necessary to set up an efficient developer environment for software engineering projects. Completing this assignment will give you the skills required to set up a robust and productive workspace conducive to coding, debugging, version control, and collaboration.

#Tasks:

1. Select Your Operating System (OS):
   Choose an operating system that best suits your preferences and project requirements. Download and Install Windows 11. https://www.microsoft.com/software-download/windows11

     What you need: Windows installation media. This could be an installation ISO or DVD.
   USB flash drive with at least 5GB free space,ensure the flash disk has nothing important since it will be formatted.
   Technician PC - Windows PC that you'll use to format the USB flash drive
   Destination PC - A PC that you'll install Windows on and then;
     Format the drive and set the primary partition as active.
     Connect the USB flash drive to your technician PC.
     Open Disk Management: Right-click on Start and choose Disk Management.
     Format the partition: Right-click the USB drive partition and choose Format. Select the FAT32 file system to be able to boot either BIOS-based or UEFI-based PCs.
     Set the partition as active: Right-click the USB drive partition and click Mark Partition as Active
 Afterwards, Copy Windows Setup to the USB flash drive.
            Use File Explorer to copy and paste the entire contents of the Windows product DVD or ISO to the USB flash drive.
        you can add an unattend file to automate the installation process.
   Finally, you Install Windows to the new PC.
    Connect the USB flash drive to a new PC.
   Turn on the PC and press the key that opens the boot-device selection menu for the computer, such as the Esc/F10/F12 keys. Select the option that boots the PC from the USB flash drive.
    Windows Setup starts. Follow the instructions to install Windows.
    Remove the USB flash drive.

2. Install a Text Editor or Integrated Development Environment (IDE):
   Select and install a text editor or IDE suitable for your programming languages and workflow. Download and Install Visual Studio Code. https://code.visualstudio.com/Download

   Download Visual Studio: Visit the Visual Studio website and click on "Download Visual Studio."
   Follow the on-screen instructions to download the installer.
   Run the Installer: Run the downloaded installer.
   Choose the "Visual Studio" workload during installation, which includes the necessary components for general development.
   Select Workloads and Components: In the Visual Studio Installer, select the workloads and components you need based on your development requirements. Common workloads include ".NET Desktop Development" or "Web Development."
   You can then Modify Installation, If needed, you can customize the installation by clicking on the "Individual components" tab in the installer and selecting or deselecting specific components.
   Install: Click the "Install" button to start the installation process.
   Launch Visual Studio: Once the installation is complete, launch Visual Studio.
   Sign in with your Microsoft account or create one if prompted.
   Choose Development Environment: On the welcome screen, select your development environment. For example, you can choose "Development Settings" based on your preferred coding style.
    Start Coding: You're now ready to start coding.
3. Set Up Version Control System:
   Install Git and configure it on your local machine. Create a GitHub account for hosting your repositories. Initialize a Git repository for your project and make your first commit. https://github.com
     
    For Windows(Since thia is the OS I'm using) Download the latest version of Git for Windows from the official website https://www.git-scm.com/downloads. Choose the 64-bit or 32-bit version depending on your system.
    Run the installer and follow the on-screen instructions. During installation, you can choose a default text editor and enable options like using Git Bash as your default terminal emulator.
    Configuring Git:
    Open a terminal window (Command Prompt on Windows, Terminal on Mac/Linux).
    Run the following commands to set your username and email address for Git commits:
                  git config --global user.name "Your Name"
                  git config --global user.email "your_email@example.com"
    Replace "Your Name" and "your_email@example.com" with your actual information.
    Creating a GitHub Account:
     Go to https://github.com/ and sign up for a free account.
     Follow the on-screen instructions to complete your registration.
    Initializing a Git Repository:
    Open a terminal window and navigate to your project directory using the cd command.
    Run the following command to initialize a new Git repository in the current directory:
             git init
   Making your First Commit:
    Create some files for your project. (These can be code files, text documents, etc.)
    Run the following command to add your project files to the staging area:
             git add .
    The . dot refers to all files in the current directory.
    Type a descriptive commit message and run the following command to commit your changes:
             git commit -m "Initial commit"
    Replace "Initial commit" with a more specific message describing your changes.

4. Install Necessary Programming Languages and Runtimes:
  Instal Python from http://wwww.python.org programming language required for your project and install their respective compilers, interpreters, or runtimes. Ensure you have the necessary tools to build and execute your code.
         Installation on Windows
Visit the link https://www.python.org/downloads/ to download the latest release ofPython. In this process, we will install Python 3.8.6 on ourWindows operating system.
  Click on the Install Now
 Double-click the executable file, which is downloaded;
Select Customize installation and proceed.
Click on the Add Path check box, it will set the Python path automatically.
Step - 1: Select the Python's version to download.
Now, try to run python on the command prompt. Type the command python -version in case of python3.

5. Install Package Managers:
   If applicable, install package managers like pip (Python).

   Download Python: Go to the official Python downloads website: https://www.python.org/downloads/.
Choose the installer: Download the latest version of Python that matches your system architecture (32-bit or 64-bit). Make sure to choose the installer that includes "add python to PATH" option. This will ensure you can run Python commands from any directory in your command prompt.
Run the installer: Double-click the downloaded installer and follow the on-screen instructions. During installation, keep the "Add Python 3.x to PATH" option checked.
   Verifying pip installation:
Once you've installed Python, use the following command to check if pip is also installed:
Bash
python3 -m pip --version

6. Configure a Database (MySQL):
   Download and install MySQL database. https://dev.mysql.com/downloads/windows/installer/5.7.html
 Secure the Installation:
After installation, run the MySQL Secure Installation script to improve security. This script sets a root password, removes anonymous user access, and disallows remote root logins. You can find instructions on running the script in the MySQL documentation: https://dev.mysql.com/doc/mysql-secure-deployment-guide/en/
Start and Manage MySQL Service:
Windows: Use the Services Management Console to start, stop, or restart the MySQL service.
 Connect to MySQL Server:
Use the MySQL command-line client to connect to the server. You'll need the username (usually root) and password you set during secure installation.
   Bash
   mysql -u root -p
Create a Database and User:
Use SQL commands to create a database for your project and a user with specific permissions to access that database. example:
SQL
CREATE DATABASE my_project_database;
CREATE USER my_project_user IDENTIFIED BY 'strong_password';
GRANT ALL PRIVILEGES ON my_project_database.* TO my_project_user;
Replace my_project_database with your desired database name.
Replace my_project_user with your desired username.
Replace strong_password with a secure password.

7. Set Up Development Environments and Virtualization (Optional):
   Consider using virtualization tools like Docker or virtual machines to isolate project dependencies and ensure consistent environments across different machines.
       

8. Explore Extensions and Plugins:
   Explore available extensions, plugins, and add-ons for your chosen text editor or IDE to enhance functionality, such as syntax highlighting, linting, code formatting, and version control integration.
 Visual Studio Code:
ESLint: Linting for JavaScript/TypeScript
Pylance: Language support for Python
Bracket Pair Colorizer: Colors matching brackets for better code readability
GitLens: Integrates Git functionality within VS Code
9. Document Your Setup:
    Create a comprehensive document outlining the steps you've taken to set up your developer environment. Include any configurations, customizations, or troubleshooting steps encountered during the process. 

#Deliverables:
- Document detailing the setup process with step-by-step instructions and screenshots where necessary.
- A GitHub repository containing a sample project initialized with Git and any necessary configuration files (e.g., .gitignore).
- A reflection on the challenges faced during setup and strategies employed to overcome them.

#Submission:
Submit your document and GitHub repository link through the designated platform or email to the instructor by the specified deadline.

#Evaluation Criteria:**
- Completeness and accuracy of setup documentation.
- Effectiveness of version control implementation.
- Appropriateness of tools selected for the project requirements.
- Clarity of reflection on challenges and solutions encountered.
- Adherence to submission guidelines and deadlines.

Note: Feel free to reach out for clarification or assistance with any aspect of the assignment.

## Welcom to ES140X

Below are set of instructions to help you effectively participate 
in this class, ES140X: Introduction to Engineering. 


### Create your GitHub account

Git is a distributed version-control system for tracking changes in sources code during software development. It is designed for coordinating work and can be used to track changes in any set of files. GitHub is a company (owned by Microsoft) that provides hosting service for software development and version control using Git. Git and GitHub are independent identities.  

All the materials for this class, including assignments, will be hosted on GitHub and use Git to track all the changes. Hence, you will need to have a GitHub account to participate in activities in this course. 

If you do not have a GitHub account, access https://github.com/ and click the “Sign Up” button on the top right of the page. You should be able to create an account by following the instructions from that site. Once you have created the account, please email Professor McCabe (c.mccabe@vanderbilt.edu) and the TA (nicholas.c.craven@Vanderbilt.Edu) your GitHub username so we can add you to the class. 

### Watch the video on Brightspace

### Requirements.txt
Save the requirements.txt file that you received via email to your ES140X folder.

### Open your terminal/shell

#### MacOS
You can open the terminal application on MacOS by either:
1. Use Spotlight search: press “Command + Space” and search for “Terminal” or
1. Open Launchpad and look for the “Terminal” app
#### Linux 
You can open the terminal application on Linux by either:
1. Press “Ctrl+Alt+T”
2. Search for “terminal” 
#### Windows
Set up your Windows Subsystem for Linux  
The following link may provide additional information if the steps below give you trouble https://docs.microsoft.com/en-us/windows/wsl/install-win10
If you have any issues during this process, please contact one of the TAs
1. Go to the cortana search bar in the bottom left of your screen and look for `Windows Powershell`
2. Open the powershell by right clicking the icon and selecting `Run as administrator`
3. Copy and paste this single line of code into the terminal that opens up. You may have to right click to paste text into your terminal. Control-V may work as well.
      `dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart`
4. Restart your computer by selecting restart from the power options in the lower left menu of your windows bar
5. Type this web address into the search bar of any web browser
    https://www.microsoft.com/en-us/p/ubuntu-2004-lts/9n6svws3rx71?rtc=1&activetab=pivot:overviewtab
6.  Select the large blue Get button to open this app entitled Ubuntu in a Microsoft Store window. Select Get again in the windows store and then Install will appear. Hit the install button. Ubuntu will be the equivalent linux terminal you will use moving forwards
7. In the same blue box, hit the Launch button that has now appeared. This will open Ubuntu for the first time on your device. It will open a black terminal window and will say “Installing, this may take a few minutes...” 
8. Enter a UNIX username once prompted. I would recommend using firstnamelastname. No capitals or other symbols are allowed.
9. Enter a password for this username. I recommend using your computer’s login password.
10. Retype the password
11. To open a new terminal in the future, just type Ubuntu into the cortana search bar and run as administrator. This will be the terminal you use to navigate directories and files in future steps.
12. In order to get into your C drive from this linux subsystem home directory, input `cd \mnt/c/Users`
13. You may have to practice moving around to find your documents and downloads folders. Play around with using `ls` to list all of the files in your current directory, `cd` to move into a named directory, and `cd ..` to move backwards one directory. You will become more familiar with this as you go through this class.

### Setting up your Anaconda environment

Anaconda is a free, open-source distribution of the Python and R programming language for scientific computing, that aims to simplify package management and deployment. In this class, we will use Anaconda to manage our Python environment. Below are short instructions to set up the Anaconda software for Mac, Linux, and Windows (using Windows Subsystem for Linux or WSL)


#### MacOS  
1. Download miniconda from: 
    https://docs.conda.io/en/latest/miniconda.html (Select the correct installer for Python 3.8, 64-bit pkg)
2. Install miniconda from the downloaded file  
3. In your terminal/shell, clone and change into the ES140X directory (where the requirements.txt file is located)  
4. If you don’t know how to do this, make sure you watch the video labeled classroom_walkthrough.mp4 from Brightspace before continuing.
5. Create and activate a new conda environment by typing in the terminal window:
    `conda create --name class37 python=3.7 -y`  
    If prompted you may need to update your conda environment and rerun the above commands.
6. When the command has successfully executed then type:  
    `conda activate class37`   
**Note:** You will need this command whenever starting up a new terminal/shell to access the class materias

7. Add relevant channels to find the packages we need to access:  
    `conda config --add channels conda-forge`
8. Install the packages in the requirement file using   
    `conda install --file requirements.txt -y`

#### Linux and Windows (Windows Subsystem for Linux)
0.   For Windows users, make sure you have set up the Windows Subsystem for Linux (WSL) for your machine. If not, you can follow the instruction in the Windows section of the “Open your terminal” above

1. Go to this link https://docs.conda.io/en/latest/miniconda.html and select the correct installer for Python 3.8 with 32-bit or 64-bit depends on your computer (use this link if you are unsure https://itsfoss.com/32-bit-64-bit-ubuntu/)
2. Right click on the correct version and select “Copy link address”
3. Open your terminal/shell and download the file with the copied link  
    `cd $HOME`
    `curl -O <The link you just copied>`
4. Once the downloads finish, type `ls` and make sure you can identify the downloaded file (should look something like “Miniconda3-***-Linux-x86_**.sh”) , then   
    `bash <The file you just download>`
5. Restart your kernel and type `conda --version` to make sure the installation finishes. 
6. Follow the same instruction for MacOS starting from step 3. 


### Accessing an assignment or class Jupyter notebook

1. Use the `cd` command to navigate to the ES140X directory.
2. Use the `ls` command to view all of the files in that directory.
3. `cd` into the cloned assignment you wish to open. If you don’t see the assignment on your local machine, watch the classroom_walkthrough.mp4 video on how to access that.
4. Type `jupyter notebook` into your terminal
5. The jupyter notebook will be open as one tab in your default browser  































If you are on a windows machine, you need to set up your windows laptop/computer with the Windows Subsystem for Linux, instructions provided below:

# This was information i sent to students this summer, so it needs a bit of editing.
# This is to set up windows subsystem for linux, and install miniconda
Also, Monday and most likely Tuesday will be onboarding days to set up your development machine. The biggest thing you can do in that regard is make sure your windows machine has enabled support for the Windows Subsystem for Linux environments. The link below will walk you through that process, depending on your internet connection it might take a little while to install. I recommend installing the ubuntu 18.X (X is a placeholder for the minor version number, it varies) linux system once you have the subsystem installed.
https://docs.microsoft.com/en-us/windows/wsl/install-win10
A link to that operating system is here.
https://www.microsoft.com/en-us/p/ubuntu-1804-lts/9n9tngvndl3q?rtc=1&activetab=pivot:overviewtab
I then recommend updating and making an account following the steps below:
https://docs.microsoft.com/en-us/windows/wsl/user-support

If you do not have a GitHub account already, you should also make one.
https://github.com

Let us know your GitHub username as well so we can add you later to the relevant teams so you have the proper permissions.

If your internet connection is slow, then i also recommend installing miniconda over the weekend, this will be installed on your ubuntu linux system you set up previously.
You first need to download the script that will install miniconda: to do that through the commandline: (the following commands are to be typed on the command line. It is in a different font for readability here)
cd $HOME;
curl -O https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
Then you can follow the instructions here:
https://conda.io/projects/conda/en/latest/user-guide/install/linux.html
The commands above complete step 1, step 2 is unnecessary, but you can do it if you like.

After that, you are pretty much good to go, aside from installing specific packages, which we will cover on monday or tuesday.
I have a Meeting at 10AM monday, and a meeting at 13:00, the 13:00 might take 2hrs, but other than that, I am available.

Aside from that, we will provide information about the shell and navigating the command line on monday. As for the rest of the schedule, we can work on that over the weekend or more define it monday. But most of this week will be onboarding activities both as a group and on your own (but we are all on slack, so you can call/message Co or myself if you have questions). We will also work on a few days/times during the week to set specific meeting times with Co and myself.

If you have other questions, or if Co or anyone else has other suggestions, feel free!

Best,
Justin




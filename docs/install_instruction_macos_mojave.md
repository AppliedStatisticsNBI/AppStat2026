
[Back to main page](../README.md)



## Installation instruction - MacOs

These instructions have been tested on a macbook pro from 2015 running the Mojave OS. 

**Important note**: These instructions are older and not actively maintained. They were left in case you prefer working with the Anaconda application rather than with VS code, 
but [these instructions](minimal_install_vscode_miniconda.md) are recommended.


### Download Anaconda3

* Go to the [anaconda website](https://www.anaconda.com/docs/getting-started/anaconda/install#macos-command-line-installer) and download the __Command line installer__ for Mac.


* In the __Launchpad__, find and click on the __Terminal__ icon.


* Once in the terminal, run the __anaconda installer__, by typing

  `bash $HOME/Downloads/Anaconda3-2019.10-MacOSX-x86_64.sh`\
    Modify the command above to match the name of the file you just downloaded.
* Scroll through the terms of the license and type `yes` to accept. You will be asked to define a path where anaconda can be installed. Feel free to use the pathname you want (we would suggest `/Users/your_username/AppliedStatistics/anaconda3/`)


* Anaconda will now install itself. At the end of the process, you will be asked if you want to initialize anaconda. __Type "No"__


* Move back to your home directory by typing `cd $HOME`. Open a file called `.bash_profile`, and type in at the bottom of the file the following line:

  `alias anaconda3=". /path/where/you/saved/anaconda3/etc/profile.d/conda.sh; conda activate base"`


* Close your terminal and reopen a new one. To run anaconda, type in the command:

  `anaconda3`

You now have to install the Python packages listed on the course website. Some of them come pre-installed with Anaconda. For those missing, this can be done either through pip or anaconda directly. An example for iminuit is given below:

### Install iminuit

* Open a new terminal. Load the anaconda environment by typing in `anaconda3`. Then type in the command:

  `conda install iminuit`

* Type `y` once the installer finds the dependencies that will be installed. You should now be able to run the applied statistics course exercises.


### Clone the Applied Statistics Repository

*  In a folder of your choice, run the command for cloning the repository:

  `git clone https://github.com/AppliedStatisticsNBI/AppStat2026.git .`


To run a notebook, make sure you activate your anaconda environment by typing `anaconda3`. You are now set to work on the notebooks!

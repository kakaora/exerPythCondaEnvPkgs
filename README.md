# Setting up Environments and Installing Packages Using Conda

## Summary of steps to complete

- [ ] Fork this repository so you have your own copy to work on.
- [ ] Clone the repository on your local machine. 
- [ ] Edit this README.md file on your machine.
- [ ] Run the Conda commands shown in the video and describe them in the table below.
- [ ] Push your changes to your GitHub repository.
- [ ] Submit a link to this GitHub repository in Canvas.

## 1. Fork & Clone this repository

* We did this in a previous assignment. Instructions are here: https://github.com/cmcntsh/exerGitPractice
* This can also be done directly in VSCode
  * Create a new folder on your machine where you want to put this repository if you don't already have one you want to use.
  * Copy the Clone or Download path for this repository from GitHub.
  * In VSCode from the command pallette (Ctrl-Shift-P) run Git: Clone
  * Paste the path into the path field which pops up
  * Select your new folder you created on your machine
  * A new folder for the repository with the repository files should be in the folder you selected showing in the Explorer window in VSCode on the left side.
  
## Edit your README.md file

* [ ] In an editor of your choice (i.e. VSCode) edit this README.md file to add the answers requested in the tables.

## Follow along with this tutorial

* Conda What and Why? (27 min): https://www.youtube.com/watch?v=23aQdrS58e0&list=PLG9A6ovzPqX6d9uWzx0UYN9pm0zzl5ofA&index=13&t=0s
  * He installs Miniconda. We will be using Anaconda. Don't install Miniconda.
  * Follow along with the rest of the tutorial.
  * Go ahead and create the environments as he creates them in the tutorial.
  * (2021 update: I recommend managing environments as shown in the new Anaconda introduction video. https://anaconda.cloud/tutorials/getting-started-with-anaconda-individual-edition%3Fsource%3Dindividual-edition-tutorial) If you want to try creating the environments using the user interface for Anaconda Navigator instead of the command line shown in the Conda What and Why tutorial, that's fine. But watch the Conda What and Why tutorial to understand some of the differences between Conda environments and other types of virtual environments available in Python.

## Conda Concepts

* [ ] Describe the Conda concepts used in the video and listed in the table below.

|   Concept   |         Description or short answer         |
|     ---     |                     ---                     |
|What is the purpose of having different environments?     |(create an isolated environment for Python projects)|
|What is the default package manager in Python?            |(pip)|
|How do you manage environments and packages in Anaconda?  |(create and remove environments, environments to use specific version of python)|
|`conda list`       |(list of packages)|
|`conda env list`       |(list of environments)|
|How do you keep your base environment unchanged?       |(can add multiple environments to your list and change your active environment)|
|What is the link to the Conda cheat sheet? (link in video notes is broken)      |(https://www.youtube.com/redirect?event=video_description&redir_token=QUFFLUhqbFM1RjdSZVdhRmRQbEo5ZlMzYVJ1a2x2T3hfQXxBQ3Jtc0tsd29BSzd4cnkteVl6QXYyTm1pWHJMTmR6YXFzOFE1d1VpYXRqNEhtSXNxbmk3elRiWVZhd0otVnhfQ0lWSXZQdl85RHRKbWhwRTNqMWNFMXNaMFlXV1FlZUk1dmk4WlZnRUxNanN6Uk03RkNPQWpkMA&q=https%3A%2F%2Fconda.io%2Fdocs%2F_downloads%2Fconda-cheatsheet.pdf)|
|`conda create --name XXXX`       |(create a new conda environment from a list of specified packages)|
|`source activate XXXX`       |(switch to the new environment that has
a different version of Python)|
|`conda install YYYY`       |(install a package (boltons) from a specific channel
(conda-forge))|
|channels in Conda       |(path or location where conda looks for packages to install)|
|`conda install -c ZZZZ YYYY`       |(install package by searching in particular channel)|
|`conda config --show channels`       |(outputs channels)|
|`conda config --add channels ZZZZ`       |(add channel to list making it highest priority)|
|conda-forge.org       |(A community-led collection of recipes, build infrastructure and distributions for the conda package manager.)|
|`source deactivate`       |(deactivate an environment)|
|`conda config --get channels`       |(Get value of the key channels from file)|

* After creating the environments he created in the video on your computer, what would the results of running the command `conda env list` look like with the da35 environment activated. Paste the output from your command prompt in the code block below.

```
#Paste your results here.
# conda environments:
#
base                  *  /Users/TheKing/opt/anaconda3
ai38                     /Users/TheKing/opt/anaconda3/envs/ai38
da35                     /Users/TheKing/opt/anaconda3/envs/da35

```
* What command would you use to remove the environments you created for this exercise from your computer?

```
#Type the command here.
conda env remove --base bio-env
conda env remove --ai38 bio-env
conda env remove --da35 bio-env
```
## 2021 Update
Python, Anaconda, and many programming languages are constantly evolving. The video Conda What and Why provides a great explanation of why you may want to use virtual environments for your Python projects, and it provides a nice demonstration of how to work in the command line. However, environment management using Anaconda Navigator is more user friently than ever. I personally will be using Anaconda Navigator to manage environments and packages since it seems easier to see what is going on using the GUI. If you haven't done so already watch the introduction to Anaconda video and pay close attention to the section on using Anaconda Navigator to create environments and install packages. https://anaconda.cloud/tutorials/getting-started-with-anaconda-individual-edition%3Fsource%3Dindividual-edition-tutorial
 
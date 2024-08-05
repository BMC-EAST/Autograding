# Python Autograders
Autograders in Python are powerful tools that automate the testing and evaluation of student code, providing efficient feedback and streamlining the grading process.

## Otter-Grader
[Otter-Grader](https://otter-grader.readthedocs.io/en/latest/index.html#) is a open-source library that enables automated testing and grading of student code, allowing for real-time feedback and flexibility in grading assignments. 

### Setting Up an Autograding Environment
Note: This was tested on a linux based machine, but should translate to a MacOS as well.  A virtual machine was set-up with this autograding environment, if you would prefer to use this virtual machine instead of setting it up on your own machine please email apivirotto@brynmawr.edu. 

1. If Conda is not currently installed, install [Miniconda](https://docs.anaconda.com/miniconda/miniconda-install/). Follow the [instructions](https://docs.anaconda.com/miniconda/miniconda-install/#installing-miniconda) for the Linux installer to [download the .sh script](https://docs.anaconda.com/miniconda/#miniconda-latest-installer-links) and run the installation. 
2. Install [nbconvert](https://nbconvert.readthedocs.io/en/latest/install.html#installing-nbconvert), [Pandoc](https://nbconvert.readthedocs.io/en/latest/install.html#installing-pandoc), and [TeX](https://nbconvert.readthedocs.io/en/latest/install.html#installing-tex).

```bash
## nbconvert
conda install nbconvert

## pandoc
sudo apt-get install pandoc

## tex
sudo apt-get install texlive-xetex texlive-fonts-recommended texlive-plain-generic
```

<ol start="3">
<li>Install <a href="https://otter-grader.readthedocs.io/en/latest/index.html#installation">otter-grader</a> using pip.</li> 
</ol> 

```bash
pip install otter-grader
```

<ol start="4">
<li>Install <a href="https://docs.docker.com/engine/install/ubuntu/#install-using-the-repository">Docker</a> with the instructions at the link (Steps 1, 2, 3). Docker is required for the local grading of assignments using containerization. </li>
</ol> 

<ol start="5">
<li>Install ipykernel. </li>
</ol> 

```bash
python3 -m pip install ipykernel
python3 -m ipykernel install --user
```

<ol start="6">
<li>Otter-grader offers a <a href="https://otter-grader.readthedocs.io/en/latest/tutorial.html">tutorial</a>. To test your installation, you can download the tutorial repository using the commands below. Basic commands to run otter-grade to test the installation are included as well. More information about <a href="#creating-and-configuring-assignments">formatting your assingments</a> and <a href="#deploying-your-autograder">Deploying the autograder for grading assignments</a> are found below. </li>
</ol> 

```bash
## download the tutorial repository
wget https://otter-grader.readthedocs.io/en/latest/_static/tutorial.zip

## test the assign function
otter assign demo.ipynb dist

## test the grading function
otter grade -n demo -a dist/autograder/demo-autorgrader_*.zip -v -ext zip submissions/zips
```

### Creating and Configuring Assignments


### Deploying Your Autograder

## nbgrader
Coming soon!

## Ok
Coming soon!
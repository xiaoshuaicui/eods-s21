# EODS-F21 Week 1 Quiz

## Part 1: Install git and Clone Course Repo

1. If you don't already have git installed, download and install git from https://git-scm.com/downloads

2. Open a command line terminal:
    - Windows: Start -> Anaconda Prompt (Anaconda3)
    - MacOS: Command+Space -> "Terminal"
    - Linux: Terminal

3.   Navigate to a folder where you keep your projects

        # Example
        $ cd /home/bgibson/proj/

4.  Clone the course repo from https://github.com/bryanrgibson/eods-s21

        $ git clone https://github.com/bryanrgibson/eods-s21.git

---


## Part 2: Install Anaconda Python, Create Environment and Create a Notebook

1. Download and install Anaconda 3 Individual Edition from https://www.anaconda.com/products/individual

    - Windows: 64-Bit Graphical Installer (457 MB)
    - MacOS: (recommended) 64-Bit Command Line Installer (428 MB)
    - Linux: 64-Bit (x86) Installer (529 MB)

    Follow the instructions here for your os: https://docs.anaconda.com/anaconda/install/
    (recommended) “Do you wish the installer to initialize Anaconda3 by running conda init?” : “yes”. 

2. Open a new command line terminal
    - Windows: Start -> Anaconda Prompt (Anaconda3)
    - MacOS: Command+Space -> "Terminal"
    - Linux: Terminal

3. Navigate to where you cloned the course repo
    
        (base) $ cd ~/proj/eods-s21

4. If you are in the base anaconda environment, you should see `(base)` in the shell prompt (see example above).
If you don't see `(base)`, activate the base environment with:
    
        $ conda activate
    
5. Create a new virtual environment using the requirements file:

        (base) $ conda create -n eods-s21 --file docs/requirements.txt

6. Activate the new environment

        (base) $ conda activate eods-s21

7. Add the new environment to jupyter

        (eods-s21) $ python -m ipykernel install --user --name eods-s21
        
8. Return to the base environment and launch Jupyter Notebook server

        (eods-s21) $ conda deactivate
        (base) $ jupyter notebook

9. In Jupyter, navigate to the folder: weekly_quiz/

10. Open a new notebook using the newly created kernel: New -> eods-s21

11. Rename the notebook "Week_01_Quiz-UNI", replacing UNI with your uniqname

12. In the first cell import pandas:

        In []: import pandas

13. In the second cell print out the version of pandas imported:

        In []: print(pandas.__version__)

---

## Part 3: Submission

1. In the notebook created above, click: File -> Print Preview

2. In the browser window, print to pdf : Print -> Save as PDF -> Week_01_Quiz-UNI.pdf, again replacing UNI with your uniqname

3. Upload pdf to Gradescope (should receive link via email)

# Zude05
GUI for creating football visualizations

# Python, Anaconda, and Jupyter Notebook Installation Guide

This guide provides step-by-step instructions for installing Python, Anaconda, and Jupyter Notebook on both macOS and Windows.

## Python Installation

### macOS

1. Open a terminal.

2. Check if Python is already installed:
   ```bash
   python --version

If Python is not installed, install it using Homebrew:
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

    brew install python

## Windows
Download the latest Python installer from the official website: Python Downloads.
Run the installer and make sure to check the box that says "Add Python to PATH" during installation.
Click "Install Now" and wait for the installation to complete.
Verify the installation by opening a command prompt and typing:

    python --version

## Anaconda Installation
**macOS and Windows**

Download the Anaconda installer from the official website: Anaconda Downloads.
Run the installer and follow the on-screen instructions.
During installation, make sure to check the box that says "Add Anaconda to my PATH environment variable."
Click "Install" and wait for the installation to complete.
Verify the installation by opening a new terminal or command prompt and typing:

    conda --version


##Jupyter Notebook Installation
**macOS and Windows**

Open a terminal or command prompt.
Install Jupyter Notebook using conda:

    conda install -c conda-forge jupyterlab

Start Jupyter Notebook by typing:

    jupyter notebook


Your default web browser should open with the Jupyter Notebook interface.
Create a new notebook or open an existing one to start working.


# Soccer Data Visualization Tool
This tool allows you to visualize soccer event data in an interactive GUI. It produces visualizations like touchmaps, passmaps, etc. for selected players.

## Requirements
The tool requires the following to run:

Python 3.x
Jupyter Notebook
Packages: tkinter, pandas, matplotlib, mplsoccer, soccerdata, socceraction
See the instructions above on setting up Python and the required packages.

## Usage
The tool expects seasonal data files to be placed in a csv folder. The files should follow this naming convention:
merged_2324_LaLiga.csv
merged_2324_LaLiga_spadl.csv

The merged_season_leaguename.csv file contains the event data. The merged_season_leaguename_spadl.csv file is optional and only needed for visualizing carries.

To get a player's Understat ID, go to their profile page on www.understat.com. The ID will be in the URL:
https://understat.com/player/99

The ID in this case is 99.

Once the data is set up, run the Jupyter Notebook and interact with the GUI to generate visualizations.

## Visualizations
The following visualizations are supported:
Touchmap, Passmap, Defensive Actions, Take-ons, Half-space and zone14 passes, Receptions, Carries, Shots.
Select the player, season, and visualization types, then click "Create Vizzes" to generate the images.

## How to use Zude05
1. Run the Zude05 Notebook file from JupterNotebook
2. Click on the Load csv button.
3. Select the Team
4. Select the Player
5. Insert the understat ID of the player if you want to visualize shots with xG.
6. Pick the Colors
7. Setup Figure and Pitch Configuration
8. Select your first colormap for the receptions and the second one for xG and xT (carries).
9. Choose your visualizations from the checkboxes.
10. Click on Create Vizzes.
11. You will find the vizzes in the Output folder. Make this directory where the Notebook is located, if it's not there already. 

## How to scrape data from whoscored
https://soccerdata.readthedocs.io/en/latest/

## Additional Resources
1. https://github.com/mckayjohns <br>
2. https://socceraction.readthedocs.io/en/latest/ <br>
3. https://mplsoccer.readthedocs.io/en/latest/

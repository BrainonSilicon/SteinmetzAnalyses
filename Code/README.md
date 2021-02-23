# CODE

This directory contains the code (in a jupyter notebook) and data for the neuropixel data analysis. 

## Code Overview :bookmark_tabs:

The code (in the notebook) has 5 sections 
- Introduction to the Project and analyses 
- Set Up 
- Data Exploration
- Spike Analyses 
- Predictive modeling, correlation analyses, and PCA

### Introduction to Project
Gives some background to the dataset and the 'why' of the chosen analyses 

### Set Up
Imports required packages
Loads in the dataset 
Runs a test to check if the data was imported 

### Data Exploration :mouse:
- Looks at what is in the data via shape and calls its keys 
- Creates a dictionary of the mice
- Finds out what brain areas the dataset has recordings from
- Creates a table of the data so that we can better visualize what's in it

### Spike Analyses :boom:
- Creates lists of the brain areas and regions that were recorded from 
- Analyses the spiking neurons in a mouse's primary visual cortex
- Analyses the spiking neurons for many mice in many regions
- Analyses the spiking rate's relationship to a presented stimuli and a corresponding motor response
- Looks at identified regions of interest and their response to the visual stimuli

### Modeling :brain:
This section contains a "decoding model" for brain data as well as some PCAs 
- Uses a Logistic Regression model on averged spiking to predict movement 
  - first for whole brain  
  - and then area by area
- Introduces using PCA dimensionality reduction instead of time avageraging (returns a [matrix](https://media.giphy.com/media/BdghqxNFV4efm/giphy.gif))
- Sets up trials based on the correctness of a movement response
- Runs a PCA on neuronal responses from the time bins closest to stimuli presentation and movement response 
  - looks at the relationship between stimuli presented and avg firing rate for each PC
  - and the relationship between movement response (right vs left vs no movement) for each PC
- Finds the correlation between a neuron's activity and a movement response
- Finds the best and worst neurons based on their correlation between activity and a movement response
- Analyses the best and worst neurons' correlation to a movement

### Bonus Analyses (because 3D plots are fun!) 
- Plots 3 identifed PC's (taken from the neuron activation level in each of the trials) in 3D 
  - Each dot represents a trial (in session 11 there were 340 trials)
  - the location is determined by the avg spiking over time (aka. activation)
  - and the dot's colours is based on the movement responses (move or not move)







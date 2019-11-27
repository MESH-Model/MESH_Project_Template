## This repository is a template for individual MESH modelling projects and contain information about a basin and modelling activities conducted using MESH.

- Each repository stored on GitHub is limited to **1 GB** (see [here](https://help.github.com/en/github/managing-large-files/what-is-my-disk-quota) for more details)
- No one file may be larger than **100 MB**
- Include large files in a .gitignore file and include a push/pull script corresponding to the storage location on a Server (e.g. Graham)
  - For more information about .gitignore files, see the GitHub manual [here](https://git-scm.com/book/en/v2/Git-Basics-Recording-Changes-to-the-Repository#_ignoring) or a repoistory with some example .gitignore files [here](https://github.com/github/gitignore).

To create a new basin repository:
1. Click "Use this template" from the MESH_Project_Template repository page

![](./UseTemplate.JPG)
2. Name the new repository "MESH_Project_<Watershed Name>" (ex. "MESH_Project_Baker_Creek")

3. Update the main "ReadMe.md" and "ProjectOverview.md" documents with project-specific information, and populate the folders.

# Project Title

## Team
  *Include the name of modeller(s), advisors, and other contributors involved in the project here, as well as key contact information*

## Date
*Date(s) of the project*

## Purpose
  *Give a brief summary of the purpose of the modelling project here*

## Objectives and Main Tasks
  *List the objectives of the modelling, as well as a summary of the project structure and tasks completed*

## Basin Meta-data
*Include a link to the MESH Wiki "Basin Meta-data" page, if created. Otherwise, link to a "Basin_Metadata.md" file in the "Site" folder

[Basin Meta-data on MESH Wiki Page](https://wiki.usask.ca/display/MESH/Basin+Meta-data) *Update to go directly to the basin page*

[Basin Meta-data File](https://github.com/HaleyBrauner/MESH_Repo_Template/blob/master/Site/BasinMetaData.md)

## Progress / Conclusion
*Include periodic updates on the modelling progress here, or even just "in progress"*
*Include the main findings of the modelling, and further recommendations*

## References
- List any scripts, packages, etc. used
- Related research papers and other information (theory, parameter selection, etc.); could include a copy in Model>Justification folder
- Manuals (ex. CLASS, Ostrich, MESH Wiki, other)

___
___
# Folder Structure
Given the file size limitations of GitHub, only smaller files are stored here and the rest are stored on Graham. The files can be synced with the local machine via the respective push/pull bash scripts included in the Data/Raw and Model folders.

Fore reference, the general rule for file sizes on GitHub is:
- Repositories should be < 1 GB
- Files must be < 100 MB

## Code
- Includes pre- and post-processing scripts used in the project

## Data

### Raw
- Includes data downloaded from ECCC using R, ESSD data (Spence & Hedstrom, 2018), GEM and CaPA data, and WSC streamflow (downloaded manually, though this should be done with an R script)

### Processed
- Includes processed driving data, spatial data (for use in Green Kenue to generate the r2c file for Scenario 3), and streamflow data used for validation

#### Driving
- Processed driving data used in the model
  - One set used for Scenario 1
  - One set used for Scenarios 2 and 3
    - Note: this is the same data as Scenario 1, but copied to 6 columns -> one per GRU
- Scripts used to generate the Scenario 1 file are included in the "Code" folder

#### Spatial
- Green Kenue files used to generate the r2c file for Scenario 3

#### Validation
- Streamflow data, including the full period, calibration period (all other values set as negative), and validation period (all other values set as negative)

## Model
*Includes "MESH Modelling Journal.docx", which is notes kept during the modelling.  
Also includes a "ReadMe.md" file which describes the differences between the model scenarios.*

### Justification
- Include an Excel (xlsx) file outlining the parameters and ranges used in the model and rationale for their use (with references listed).
- Also includes the equation used in scaling wind observations from near-surface to reference height (which was 40m)

### MESH_Code
- Holds the MESH code used for running the mode
  - MESH_Code.r1024 was used for Scenarios 1, 2, and 3 of the modelling project
  - r1552_mod was used for Scenarios 1-P and 2-P
  - No modifications were made to the code

### Ostrich
- This folder contains a copy of the Ostrich program (uncompiled).

### Scenario_*
*1 folder for each configuration, each with input and output sub-folders*

- Input  
  - *Includes the MESH inputs files, driving data, and scripts for the model configuration*

- Output
  - *Includes the output files for the model configuration / each run*

## Presentations
*Contains the final powerpoint presenation and the draft project report (final pdf yet to be released)*

## Site
Includes:
- Maps
- PhotosVideos
- Site Meta-data

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

[Basin Meta-data on MESH Wiki Page](https://wiki.usask.ca/display/MESH/Basin+Meta-data)

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
## Folder Structure

### Code
*Includes pre- and post-processing scripts used in the project*

### Data

#### Driving
Raw
- Met data, streamflow, station metadata, soil moisture/temp, etc.
- Subfolder for each type/source

Spatial
- Green Kenue files
- GIS files

Validation
- ex. streamflow

### Model
*Include model notes in this main "Model" folder, as available*

MESH_Code
- Holds the MESH code used for running the mode; use a new folder for each version (include the version as a suffix)
- If any modification of the code were made, or more than one version was used, include a text file listing the MESH code versions, the main differences and reason for use, and details of the modifications

ConfigurationX
*Include 1 folder for each configuration, with input and output sub-folders*

- Input *(Includes the MESH inputs files, driving data, and scripts for the model configuration)*

- Output *(Includes the output files for the model configuration / each run)*

Justification
*Includes files related to scenario configuration choice, parameter selection, initial conditions, etc.*

Superceded
*Include previous versions of certain files only if relevant to the project*

Presentations
*Contains powerpoint (or similar), poster, or other presentations or reports related to the project (formal or otherwise)*

### Site
- Maps
- PhotosVideos
- Reports
- Site Meta-data

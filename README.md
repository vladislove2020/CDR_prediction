# CDR_prediction
Demo Jupyter notebook for my kursach

Welcome to the demonstration code for my university annual project (:

The aims of my project were:
 - to prepare dataset of structures and information about antibodies binding to COVID-19 spike protein RBD epitope
 - to perform automated prediction of CDRH3 and CDRL3 loops backbones via RFDiffusion
 - to perform automated prediction of CDRH3 and CDRL3 loops sequences based on predicted backbones via ProteinMPNN
 - to analyze and visualize results of such prediction

I express my gratitude to the authors of used tools:
 - RFDiffusion : https://github.com/RosettaCommons/RFdiffusion
 - ProteinMPNN : https://github.com/dauparas/ProteinMPNN

In main.ipynb you will find all the code I used for the project

If you want to launch code at your own, you will need to prepare some python environments:
 - Python 3 environment with IPykernel to launch the code in main.ipynb (versions of used libraries are in requirements.txt file)
 - environment for RFDiffusion version 1.1.0 (all instructions are in RFDiffusion GitHub repo)
 - environment for ProteinMPNN version 1.0.1 (all instructions are in ProteinMPNN GitHub repo)

Note that RFDiffusion and ProteinMPNN are launched in terminal (main.ipynb contain cells automatically creating shell scripts for this, but you should then execute these scripts manually through the terminal in corresponding environment)

Folder visualization_examples contains some subfolders of the working directory I got after launching all the code in main.ipynb:
 - global_vis : plots of distributions of RMSDs and sequence alignment scores with wild-type variant for individual predictions
 - ramachandran_maps : Ramachandran maps representing torsion angles in predicted loops
 - pymol_vis : pictures and PyMOL session files for designed loops superposed on the wild-type variant

I express my gratitude to the authors of PyMOL, software I used to make molecule visualization : https://pymol.org

Pictures of the structures were generated with default camera angle, so you can open in PyMOL corresponding .pse files, manually rotate camera and make your own pictures

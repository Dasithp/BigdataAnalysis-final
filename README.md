# Final-Project
This repository contains all the files I used in order to complete my final big data analysis assignment.

My research proposal includes looking at the serum microbiome of diabetics with periodontitis and comparing it to diabetics without periodontitis and normal, healthy subjects.
The focus of my assignment is to test the methodology that I propose to carry out for this project. In order to test this method I used some publically available data that looked at the microbiome in the plasma component of blood, compared to the buffy coat layer and red blood cell layer.

The raw illumina sequence data that I used for this purpose exceeded the 1000MB file limit of github (despite it being a compressed file). The data can be found either by contacting me or may be obtained from https://www.ncbi.nlm.nih.gov/pubmed/26865079 
For the purpose of this project I only used the forward reads listed in the r1 folder for both the buffy coat and plasma

I carried out quality control using trimmomatic and flexbar. I used fastqc to verify the quality

I used MED to cluster the sequences and largely obtain species level resolution.
The Human Oral Microbiome database was used to label the species that match the output of MED. For the purpose of this assignment, I used the top hit on HOMD for each of the calls. So it is important to note that the species mentioned in the document may not be their true identities but rather their closest relatives as based on the HOMD database.

The MED and HOMD alignment result files can be found in the "MEDoutput" folder.
   
The file containing my proposal is titled as "Big data Proposal" and is a pdf document.

The file "Blood microbiome Plasma vs buffy coat.ipynb" is a jupyter notebook and contains all the work that I did in order to obtain my results.

The files "plasmabc.csv" and "plasmabc.txt" are the files required for LefSe analysis. plasmabc.csv was obtained via my workflow listed in "Blood microbime Plasma vs buffy coat.ipynb". plasmabc.txt is just a file conversion as this format is what is required by LeFse analysis.    

I wrote my proposal using MS word and converted the file into a PDF, both files are part of this repository


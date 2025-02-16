# MINT - Metabolomics Integrator
MINT is a post-processing tool for _liquid chromatography-mass spectrometry_ (LCMS) based _metabolomics_. 
Metabolomics is the study of all metabolites (small chemical compounds) in a biological sample e.g. from bacteria or a human blood sample. 
The metabolites can be used to define biomarkers used in medicine to find treatments for diseases or for the development of diagnostic tests 
or for the identification of pathogens such as methicillin resistant _Staphylococcus aureus_ (MRSA). 

![Flowchart of MINT workflow](image/flowchart.png "Flowchart of MINT workflow")<br/>
_**Figure 1:**_ Flowchart of MINT processing workflow. 



## How to use MINT?
The tool can be used for targeted analysis where the m/z-values (mass to charge ratios) and chromatographic retention times are known. 
Alternatively, MINT can be used in an untargeted approach where new biomarkers can be explored without prior knowledge.

MINT currently supports the open data formats mzML and mzXML. The main function is to extract and characterise measured 
intensities in a given m/z and retention time (RT) window. These windows can be provided in form of a [peaklist](peaklists.md) 
or created interactively in the [GUI](gui.md). With this setup large numbers of LCMS-files can be processed automatically, 
standardized and perfectly reproducible.

The tool can be used with a browser based graphical user interface (GUI) implemented as interactive dashboard with 
[Plotly-Dash](https://plot.ly/dash/). Alternatively, the `ms_mint` package can be imported as python library to be 
integrated in any regular Python code as part of a larger processing pipeline or interacively in the [Jupyter Notebook](jupyter.md).

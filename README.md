# dual-task-metacognition-data

Manuscript: When Dual-Task Costs Extend to Metacognition: Evidence From Modality Overlap

1. Archive Contents

The archive is organized into four experiment folders: Exp1, Exp2, Exp3, and Exp4. Each folder contains raw data, participant-level analysis data, a Python data extraction script, an SPSS data file, SPSS analysis syntax, and statistical output.

Additional files:
DATA_DICTIONARY.txt: Variable definitions, condition codes, and calculation methods for the main measures.

Participant IDs are specific to each experiment. Identical IDs across experiments do not indicate the same participant.


2. File Structure

Exp1 is shown below as an example; the other experiment folders follow the same structure.

Exp1/Exp1data/: Raw event records and trial-level CRT data in CSV format.
Exp1/Exp1_extract.py: Python script for extracting analysis variables from the raw CSV files.
Exp1/Exp1_analysis.csv: Participant-level analysis data.
Exp1/Exp1_analysis.sav: Corresponding SPSS data file.
Exp1/Exp1_syntax.sps: SPSS analysis syntax.
Exp1/Exp1_Results.pdf: SPSS statistical output.


3. Data Extraction

The extraction scripts use Python 3 and require only the standard library; no third-party packages are needed. The scripts were previously run using Python 3.6.6.

Run the following commands from the project root directory:

python Exp1/Exp1_extract.py
python Exp2/Exp2_extract.py
python Exp3/Exp3_extract.py
python Exp4/Exp4_extract.py

Each script reads the raw data for the corresponding experiment and generates ExpN_analysis.csv. Rerunning a script overwrites the existing output file.

See DATA_DICTIONARY.txt for variable definitions, condition codes, and calculation details.


4. SPSS Analyses

Analysis syntax is provided in the corresponding ExpN_syntax.sps file, and statistical output is provided in ExpN_Results.pdf.

The SPSS data files include a filter variable for selecting the analysis sample. The exclusion criteria and final sample size for each experiment are reported in the manuscript. Apply the exclusions described in the manuscript when reproducing the statistical analyses.

The .sav files provide the analysis data in SPSS format and are not automatically updated by the Python extraction scripts.

SPSS version used: IBM SPSS Statistics (Version 27).

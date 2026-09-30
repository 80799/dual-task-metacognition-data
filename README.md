# dual-task-metacognition-data

Manuscript: When Dual-Task Costs Extend to Metacognition: Evidence From Modality Overlap


1. Archive Contents

The archive is organized into four experiment folders: Exp1, Exp2, Exp3, and Exp4. Each folder contains raw data, experimental task files, participant-level analysis data, a Python data-processing script, an SPSS data file, SPSS analysis syntax, and statistical output.

Additional file:
DATA_DICTIONARY.txt: Variable definitions, condition codes, units, and calculation methods for the main measures.

Participant IDs are specific to each experiment. Identical IDs across experiments do not indicate the same participant.


2. File Structure

Exp1 is shown below as an example; the other experiment folders follow the same structure.

Exp1/
    Exp1_raw_data/
        Raw experimental data files.

    Exp1_task_program/
        Experimental task files used to run the study.

    Exp1_analysis.csv
        Participant-level analysis dataset in CSV format.

    Exp1_analysis.sav
        Corresponding participant-level analysis dataset in SPSS format.

    Exp1_data_processing.py
        Python script used to process the raw data and generate Exp1_analysis.csv.

    Exp1_syntax.sps
        SPSS syntax used for the statistical analyses reported in the manuscript.

    Exp1_results.pdf
        SPSS statistical output corresponding to the reported analyses.


3. Data Processing

The data-processing scripts use Python 3 and require only the Python standard library; no third-party packages are needed. The scripts were previously run using Python 3.6.6.

Run the following commands from the project root directory:

python Exp1/Exp1_data_processing.py
python Exp2/Exp2_data_processing.py
python Exp3/Exp3_data_processing.py
python Exp4/Exp4_data_processing.py

Each script reads the raw data files in the corresponding ExpN_raw_data folder and generates ExpN_analysis.csv. Rerunning a script overwrites the existing CSV output file.

The resulting CSV files contain the participant-level variables used in the statistical analyses. See DATA_DICTIONARY.txt for variable definitions, condition codes, units, and calculation details.


4. Statistical Analyses

Statistical analyses were conducted using IBM SPSS Statistics (Version 27).

For each experiment, the SPSS analysis syntax is provided in ExpN_syntax.sps, and the corresponding statistical output is provided in ExpN_results.pdf.

The ExpN_analysis.sav files contain the participant-level analysis data in SPSS format. These files correspond to the analysis datasets but are not automatically regenerated when the Python data-processing scripts are run.

The SPSS data files include a filter variable for identifying the analysis sample. Participant exclusion criteria and final sample sizes are reported in the manuscript. The same exclusions should be applied when reproducing the reported statistical analyses.


5. Experimental Materials

The ExpN_task_program folders contain the experimental task files and associated materials used for each experiment. These files document the task structure, stimulus presentation, trial sequence, response collection, and other procedural details required to reproduce the experimental procedure.

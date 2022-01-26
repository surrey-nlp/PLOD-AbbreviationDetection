This folder contains the file PLOD_dataset-filtered-validated.zip, which contains only one file: PLOD_dataset-filtered-validated.tsv.

PLOD_dataset-filtered-validated.tsv contains 11 columns separated by tabs and 160,932 rows. Here is a description of what each of the columns means:

- Column 1 = Segment ID
- Column 2 = Segment Text
- Column 3 = Indexes of the Abbreviations in the segment
- Column 4 = Indexes of the Long Forms in the segment
- Column 5 = Abbreviations (extracted based on the indexes from column 3)
- Column 6 = Long Forms (extracted based on the indexes from column 4)
- Column 7 = Name of the file in the PLOS corpus
- Column 8 = Name of the folder in the PLOS corpus (= name of the PLOS Journal)
- Column 9 = Automatic validation (further explained below)
- Column 10 = Abbreviations (as they appear in the "Abbreviation" section of the XML from the corpus) -- this column is just for reference
- Column 11 = Long Forms (as they appear in the "Abbreviation" section of the XML from the corpus) -- this column is just for reference

Validation (column 9 in PLOD_dataset-filtered-validated.tsv). This column contains either a 1, a 2, a concatenation of both, or it is empty.
- If it contains a 1, at least one of the long forms in this line begins or ends with a stop word.
- If it contains a 2, at least one of the long forms in this line has more than 12 tokens.
- If it contains any concatenation of 1 and 2 (either 12 or 21), then both the above are true.
- If it is empty, then none of the above are true.

Problem Understanding: Asked Redrob to explain the 
full 7-step pipeline and identify the most critical step. 
Redrob identified normalization as critical because errors 
there cascade into all downstream computations.

Normalization and Deduplication: Asked Redrob to 
write normalize_and_deduplicate_skills() with multi-word phrase 
matching before single tokens and order-preserving deduplication. 
Validated all 10 candidate outputs against expected results before 
proceeding.

Vocabulary and TF-IDF: Asked Redrob to build shared 
vocabulary from resume skills only (48 terms, alphabetically 
sorted), compute df_map, and generate TF-IDF vectors using 
TF=1/N and IDF=ln(10/df). Verified df values matched expected: 
python=6, machine_learning=3, data_visualization=3.

JD Vectors, Cosine Similarity and Rankings: Asked 
Redrob to normalize JD skills through SKILL_ALIASES, build binary 
vectors over same vocabulary, compute cosine similarity for all 
10 resumes x 3 JDs, and output top 3 per JD with tie-breaking.

Final Integration: Asked Redrob to combine all stages 
into one clean file with import math at top, clear stage comments, 
all intermediate outputs printed, and correct final format.

At each stage I validated intermediate outputs before moving to 
the next prompt. This caught df computation errors and JD 
normalization issues early.

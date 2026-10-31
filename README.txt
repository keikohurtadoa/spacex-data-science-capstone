SpaceX capstone: seven completed notebooks

Open the .ipynb files in Jupyter Notebook, JupyterLab or Google Colab.
Run the cells from top to bottom. Completed outputs are saved in the notebooks.
Original task numbering is retained (the final notebook is numbered 8).

01 - API data collection
02 - Wikipedia web scraping
03 - Data wrangling and landing labels
04 - SQL analysis (using built-in sqlite3)
05 - Data visualization and feature engineering
06 - Launch-site maps and approximate distances
08 - Machine learning, tuning, accuracy comparison and confusion matrices

Important notes:
- The live SpaceX API returned a server error during verification. Notebook 01
  includes the API solution and an explicit fallback to IBM's prepared course
  dataset. Its saved results use that fallback; payload masses in it are already
  imputed. It does not represent a fresh live API extraction.
- Notebook 02 uses the historical Wikipedia page specified by the assignment.
- Notebook 06 distances use approximate selected reference coordinates, not
  computed nearest points or driving distances. The saved HTML map needs internet
  access to load base-map tiles.
- Notebook 08 demonstrates scaling in Task 2, then evaluates models using
  unscaled splits and scalers fitted within each cross-validation training fold.
  The deprecated decision-tree max_features='auto' is replaced with None.
  All four models tied at 83.33% test accuracy in this run. Cross-validation
  preferred the decision tree. The test set has only 18 observations.

The CSV outputs and interactive HTML map are included as supporting files.

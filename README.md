# **Weekly Asssessment:** *Data Exploration and Visualizations for Census Annual Business Survey*
### **Contributors:** Tavianne Kemp, Jack Lynn, Stanley Perez, & Sam Wainright

### **Essential Questions**

1. What demographic disparities exist in the American workforce?
2. What demographics are disproportionately negatively affected?

### **Summary**

Because of historical inequity and persisting racism, misogyny, and xenophobia, **the United States job market disadvantages certain ethnic, racial, and sex groups**. This data exploration project uses the [**Census's Annual Business Survey (ABS)**](https://www.census.gov/data/developers/data-sets/abs.2019.html) to explore these disparities and **characterize the demographic trends of the US job market**. First, the data is imported through **Census APIs** and **transformed using a specified ETL process (`etl.ipynb`)**. Second, the data is **transformed** and **graphically depicted** to characterize ethnic, racial, and sexual disparities in business ownership and employeeship. Third, findings are summarized in three reports, one **PowerPoint presentation** (`presentation.pptx`), one **ETL** document (`etl.docx`), and one **report** (`report.docx`) (*See the `reports` directory*).

### **Datasets**

*All datasets are imported into the ETL document (`etl.ipynb`) through APIs.*

**[Summary Dataset](https://api.census.gov/data/2018/abscs.html):** contains essential data regarding sex, race, veteran status, and ethnicity differences in employment and the US workforce; part of ABS

**[States Dataset](https://api.census.gov/data/2018/abscs.html):** same as the Summary dataset except on a state-grain; part of ABS

**[Owner Dataset](https://api.census.gov/data/2018/abscbo.html):** contains data regarding business ownership related to industry, race, sex, ethnicity, and veteran status; part of ABS

**[Demographic Dataset](https://www.census.gov/quickfacts/fact/table/US/PST045221):** contains data regarding proportion of US racial and ethnic population groups; part of QuickFacts

### **File Structure**

**`etl.ipynb`:** ETL implementation with API connections, data cleaning, and storing. Requires the use of `config.py` that is not saved with the GitHub repository; please contact Jack Lynn (jackrlynn@gmail.com) to get `config.py` file.

**`visualizations.ipynb`:** Contains four sets of graphical representations of overall, racial, ethnic, and sexual trends in the US job market. Does not require `config.py` so long as data is properly stored in `data` directory.

**`data`:** Directory location of data products of the ETL process, saved as CSV files.

**`reports`:** Directory location of reports interpreting graphical visualizations

### **How to Run**

**Pre-requisites:** Requires Python 3.8 or later, Conda environment, and Jupyter notebook interpreter.

1. Fork this GitHub directory and save to harddrive.
2. Run the `etl.ipynb` in your Jupyter notebook interpreter to form cleaned data files, saved in `data` as CSV files. This step may not be necessary because the data is already cleaned, saved, and pushed in the `data` directory with the GitHub repository.
3. Run the `visualizations.ipynb` in your Jupyter notebook interpreter to get graphical visualizations and see how the data is analyzed.
4. Read reports stored in `reports` document to get interpretation of data. The ETL document describing the importing and cleaning process is also stored here.
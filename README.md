# HSLU Project: Computational Language Technologies 
Contains the NLP project for the "Detecting greenwashing signals through a comparison of ESG reports and public media" challenge.
The analyzed datasets can be downloaded from the following Google drive:
https://drive.google.com/file/d/1D1qOuJvQx69afYyz4rwf2C-Nm0D4goKy/view?usp=sharing

Further information to the challenge/project can be found in the document in */docs* or the following links:
- https://www.swisstext.org/shared-task-1-detecting-greenwashing-signals-through-a-comparison-of-esg-reports-and-public-media/
- https://sites.google.com/view/greenwashingswisstext/home?authuser=0

### Run the analysis / EDA
- Clone the repository
- Download the data files to the */data* directory
- Install the requirements
- Run the preprocessing notebook (*stage1/00-data-preprocessing.ipynb*)
- Run the analysis notebook (*stage1/01-data-exploration-and-visualization.ipynb*)


### Repository structure
```
hslu-nlp/
┣ data/
┃ ┣ checkpoints/
┃ ┣ .gitkeep
┃ ┣ dax_company_sectors.csv
┃ ┣ esg_documents_for_dax_companies.csv
┃ ┗ sdg_descriptions_with_targetsText.csv
┣ docs/
┃ ┗ SwissText Shared Task 2023 - Greenwashing Detection.pdf
┣ stage1/
┃ ┣ 00-data-preprocessing.ipynb
┃ ┗ 01-data-exploration-and-visualization.ipynb
┣ stage2/
┃ ┣ annotated/
┃ ┣ checkpoints/
┃ ┗02-data-annotation.ipynb
┣ stage3/
┣ stage4/
┣ stage5/
┣ .gitignore
┣ README.md
┗ requirements.txt
 ```

Developed and authored by: Tim Giger
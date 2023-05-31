# HSLU Project: Computational Language Technologies 
Contains the NLP project for the "Detecting greenwashing signals through a comparison of ESG reports and public media" challenge.
The analyzed datasets can be downloaded from the following Google drive:
https://drive.google.com/file/d/1D1qOuJvQx69afYyz4rwf2C-Nm0D4goKy/view?usp=sharing

Further information to the challenge/project can be found in the document in */docs* or the following links:
- https://www.swisstext.org/shared-task-1-detecting-greenwashing-signals-through-a-comparison-of-esg-reports-and-public-media/
- https://sites.google.com/view/greenwashingswisstext/home?authuser=0

The project is structured in different stages. For each stage, the development artifacts are stored in the respective folders (e.g. stage1)

### Run the analysis / EDA
- Clone the repository
- Download the data files to the */data* directory
- Install the requirements
- Run the preprocessing notebook (*stage1/00-data-preprocessing.ipynb*)
- Run the analysis notebook (*stage1/01-data-exploration-and-visualization.ipynb*)

### Stage 1
Contains text pre-processing, cleaning and enrichment (*00-data-preprocessing.ipynb*).
After the pre-processing, an Exploratory Data Analysis was conducted (*01-data-exploration-and-visualization.ipynb*)

### Stage 2
A "gold standard" of 1'000 manually annotated (positive, negative, neutral) sentences was created.
Several LLMs were evaluated and tested with different prompting strategies. Afterward one model was selected to annoate/segment all sentences.
See *02-data-annotation.ipynb* for the full code and explanations. The manually annotated and LLM annotated dataset is stored on Google Drive:
https://drive.google.com/drive/folders/1ATtCPPll6n_qvfMBu4ka84E3DZDS7d11

### Stage 3
Based on the data annotated in stage 2, a sentiment analysis classifier was trained and evaluated. The classifier outputs scores
on a continuous scale between 0 and 1. After training, the classifier was used to predict/classify sentiment of sentences in the full data set.
Finally, the average sentiments of internal vs. external were compared to determine whether greenwashing patterns are present or not.

### Stage 4
Relevance of specific SDGs to the different companies are determined. A sentence embedding approach was used on the SDG descriptions and the
documents related to a company to compare them in terms of similarity. Finally, the results of the sentence embedding analysis were displayed
in heatmaps and bar charts to represent the SDG relevance for the different companies.

### Stage 5
A project report containing key findings and methodology of stages 1 to 4 was written.

### Repository structure
```
hslu-nlp/
┣ data/
┃ ┣ checkpoints/
┃ ┣ .gitkeep
┃ ┣ esg_documents_for_dax_companies.csv (Download the dataset and place it here)
┃ ┗ sdg_descriptions_with_targetsText.csv (Download the dataset and place it here)
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

Stage 1 & 2 developed and authored by: Tim Giger  
Stage 3, 4 & 5 developed and authored by: Arian Contessotto, Levin Reichmuth & Tim Giger
